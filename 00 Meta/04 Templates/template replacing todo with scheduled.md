<%*
const selection = tp.file.selection();
if (selection) {
const replace = selection.split("\n").map(select => {
    if (select.includes("- [ ]")) {
        select = select.replace("[ ]", "[>]");
    }
return select;
}).join("\n");
tR += replace;
} else {
    new Notice("Text must be selected");
};
%> 