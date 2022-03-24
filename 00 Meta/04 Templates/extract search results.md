<%*
//v0.2 - bug fix: when search results match just a file name and no line contents under it

//User can set the following two parameters
const resultFilePrefix = '## ';
const folderLocation = '/search';

const search = app.workspace.getLeavesOfType("search")[0];
const searchTerms = search.view.getQuery();
const arrCount = Array.from(search.view.dom.resultDomLookup);
if (arrCount.length > 0) {
    //search.view.setCollapseAll(true);
    //search.view.setCollapseAll(false);
    //search.view.setExtraContext(true);
    let resultCtr = 0;
    let finalResultString = '';
    search.view.dom.resultDomLookup.forEach(eachResult => {
        let mdCache = app.metadataCache.getFileCache(eachResult.file);
        //console.log(mdCache);
        let fileContent = eachResult.content;
        finalResultString += resultFilePrefix + '[' + `[${eachResult.file.basename}]]\n\n`;
        let results = eachResult.result.content;
        let foundStart;
        if(results) {
            results.forEach(eachItem => {
                //Check if is a list item
                let mdListItems = mdCache.listItems;
                let foundResult = false;
                if(mdListItems) {
                    mdListItems.forEach(eachList => {
                        if(eachList.position.start.offset <= eachItem[0] && eachList.position.end.offset >= eachItem[1]) {
                            foundResult = true;
                            if(foundStart != eachList.position.start.offset) {
                                let finalResult = fileContent.substring(eachList.position.start.offset, eachList.position.end.offset);
                                finalResultString += finalResult + '\n\n';
                                foundStart = eachList.position.start.offset;
                                resultCtr++;
                            }
                        }
                    })
                }

                if(!foundResult) {
                    let mdSections = mdCache.sections;
                    if(mdSections) {
                        mdSections.forEach(eachSection => {
                            if(eachSection.position.start.offset <= eachItem[0] && eachSection.position.end.offset >= eachItem[1]) {
                                foundResult = true;
                                if(foundStart != eachSection.position.start.offset) {
                                    let finalResult = fileContent.substring(eachSection.position.start.offset, eachSection.position.end.offset);
                                    finalResult = finalResult.replaceAll('#', '`#`');
                                    finalResult = finalResult.replaceAll('---', '`---`');
                                    finalResultString += finalResult + '\n\n';
                                    foundStart = eachSection.position.start.offset;
                                    resultCtr++
                                }
                            }
                        })
                    }
                }
            })
        }
    })
    
    if(resultCtr > 0 && finalResultString != '') {
        let newFileName = "SEARCH_" + tp.date.now('YYYY_MM_DD_hhmmss') + " - " + searchTerms;
        newFileName = newFileName.replace(/[\.#\*"\/\\<>\:\|\[\]\?]/gim, '').trim().slice(0, 255);
        //let vaultRootPath = app.fileManager.getNewFileParent().path;
        let bSearchFolder = await app.vault.adapter.exists(folderLocation, false);
        if(!bSearchFolder){await app.vault.createFolder(folderLocation);}
        let newFilePath = folderLocation + '/' + newFileName + ".md";
        let newFileObj = await app.vault.create(newFilePath, finalResultString);
        await app.workspace.openLinkText(newFileObj.basename, newFileObj.path, true);
    }
    //app.workspace.revealLeaf(search);
} else {
    //console.log('No search results');
}
%>