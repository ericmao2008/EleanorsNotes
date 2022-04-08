> [!INFO] Creation Steps
> Intended for publication with [[Obsidian Roundup]]
> - [Obsidian Updates](https://forum.obsidian.md/c/announcements/13) (check pins in `#mobile`)
> - [Github Action](https://github.com/argenos/obsidian_roundup/actions)
> -  [Updates channel sanitized](https://zhout-public-downloadable.s3.amazonaws.com/obsidian/updates.md) 
> - [Starboard channel sanitized](https://zhout-public-downloadable.s3.amazonaws.com/obsidian/starboard.md)
> - [Plugin Database](https://obsidian-plugin-stats.vercel.app/updates)
> - Bookmarks
> - [Feature Requests](https://forum.obsidian.md/c/feature-requests/8)
> -  [Hub merges](https://github.com/obsidian-community/obsidian-hub/pulls?q=is%3Apr+is%3Amerged+sort%3Aupdated-desc+-label%3A%22scripted+update%22+-label%3A%22hub+tools+%26+scripts%22+%3E+)

## In The Community

* The next community talk, "Easy automated testing for Obsidian plugin developers: find broken things before your users do...", is in an hour or so (9:30 AM EST). More details and a link to the zoom meeting are in [Discord](https://discord.gg/obsidianmd?event=955086222261383238). 
- Nicole van der Hoeven and Jeremy Valentine (`@javalent` is the developer of the "TTRPG suite" of plugins like dice roller, leaflet, admonitions, etc) are going to be [live on Youtube](https://www.youtube.com/watch?v=2Jm5lZWy-0Y) in a couple of hours (1pm EST) to discuss his plugins & potentially some upcoming ones 👀 

## Plugin News

### New in Community Plugins

*These plugins went through code review and are now available in Obsidian's plugin list.* For the full list, check out the [plugin stats page](https://obsidian-plugin-stats.vercel.app/new). 

- [Fleeting Notes Sync](https://github.com/fleetingnotes/fleeting-notes-obsidian) by `@matthewwong525`  this is a plugin to sync the [Fleeting Notes browser extension](https://fleetingnotes.app/) with Obsidian 
- [JiraIssue](https://github.com/marc0l92/obsidian-jira-issue) by `@marc0l92`  lets users track the progress of Atlassian Jira issues from your Obsidian notes. 
- [AsciiDoc Blocks Plugin](https://github.com/juracy/obsidian-asciidoc-blocks) by `@juracy`  renders asciidoc blocks (specifically tables)
- [Smort](https://github.com/SmortApp/obsidian-smort) lets you easily edit, annotate and share articles; the plugin brings them into Obsidian. 
- [Path Title](https://github.com/jdeal/obsidian-path-title-plugin) by `@jdeal`  adds the path (or optional replacement) to the filename title of each pane. 

### Pending (as of Friday morning)

_Note: Not all new plugins are available in the community list yet, as they need to go through code review first. You can manually install plugins that aren't in the community list yet by using the [Beta Reviewer's Auto-update Tool](https://github.com/TfTHacker/obsidian42-brat). Note, though, that this is not as safe as waiting for them to go through code review._

- [Better CodeBlock](https://github.com/stargrey/obsidian-better-codeblock) by `@stargrey`  adds titles and line numbers to Obsidian code block. Might be especially useful used in conjunction with...
- [Execute Code](https://github.com/twibiral/obsidian-execute-code) by `@twibiral` lets users run javascript code snippets from a code block. Python and Java are on the roadmap. 
- [Daily notes opener](https://github.com/reorx/obsidian-daily-notes-opener) by `@reorx`  adds some nice styling and functionality to daily notes.
- [Obsidian Google Tasks](https://github.com/YukiGasai/obsidian-goole-tasks) by `@YukiGasai`  lets users interact with your Google Tasks from inside Obsidian 
- [Latex Suite](https://github.com/artisticat1/obsidian-latex-suite) by `@artisticat1` is designed to make typing LaTeX faster through text expansion. 
- [Doubleshift](https://github.com/Qwyntex/doubleshift) by `@Qwyntex`   lets users open the command palette by pressing Double Shift like in IntelliJ 
- [List Modified](https://github.com/franciskafieh/obsidian-list-modified) by `@franciskafieh` links all modified files meeting certain criteria to a daily note. 

### Updates

 _If you want a comprehensive list of what plugins updated this week, check out this [plugin updates index](https://obsidian-plugin-stats.vercel.app/updates) by Ganessh Kumar._

* The [Tasks](https://github.com/schemar/obsidian-tasks/releases/tag/1.5.0) plugin got a big update involving recurrence, file name handling, improved documentation, support for comments inside task blocks, and more. This is a really heartwarming example of community work; 12 (!) new people made their first contributions to the plugin for this update to happen :) 
* [Custom Frames](https://github.com/Ellpeck/ObsidianCustomFrames/releases/tag/2.2.1) now has presets for Google Calendar & Todoist  
* the [Quartz publish alternative option](https://github.com/jackyzha0/quartz/releases/tag/v3.2) now supports CJK & RTL, LaTeX, and wikilinks. 
* [Another Quick Switcher plugin](https://github.com/tadashi-aikawa/obsidian-another-quick-switcher/releases/) added filename recent search. 
* The [vimrc plugin](https://github.com/esm7/obsidian-vimrc-support) now lets users define Vim commands with Javascript snippets.
* [Zotero Desktop Connector](https://github.com/mgmeyers/obsidian-zotero-desktop-connector/) got a breaking change:  users can now search for template files instead of having to type them in, but may need to re-set the templates. 
* [Code Editor Shortcuts v1.7.0](https://github.com/timhor/obsidian-editor-shortcuts/releases/tag/1.7.0) now supports multiple cursors for most commands. 
* The [Search on Internet](https://github.com/nhaouari/obsidian-search-on-internet) plugin now lets you show results in hover popups, and has better hotkeys. 
* The [Topic Linking plugin](https://github.com/liammagee/obsidian-topic-linking/) now has improved handling of larger PDF files, image handling and Zotero metadata (handled similarly to the bibnotes plugin, via a Zotero Better BibTex JSON export). The PDF output is very fiddly, and won't suit everyone's needs, but might be useful to people who are looking for Obsidian-searchable PDFs (among other things).

### Betas

_Note: these plugins have not yet been submitted for code review, and are being made available primarily for testing purposes._

* [Auto Updated Date](https://github.com/scambier/obsidian-auto-updated-date) adds a front matter updated field to your notes that is updated to the current date and time whenever you save a note.
* [Smart Link](https://github.com/jack-song/smart-link) is an experimental plugin that recommends notes that could be linked. It requires setting up dev lab server.  

### For Developers

* `@shabegom` is looking for maintainer(s) for the [block ref counter plugin](https://github.com/shabegom/obsidian-reference-count). 
* `@MSzturc`, the developer of [Advanced Slides](https://github.com/MSzturc/obsidian-advanced-slides) is [looking for a front-end developer to help](e the UI. 

## Feature Requests

* It would be neat if we could link to [callout titles](https://forum.obsidian.md/t/link-to-callout-heading/35401) the same way we can link to section headings. 

## Appearance

* [Minimal 5.1.11](https://github.com/kepano/obsidian-minimal/releases/tag/5.1.11) got a few more style settings, like the ability to disable sidebar relationship lines. 
* [Shimmering Focus](https://chrisgrieser.github.io/shimmering-focus/) reorganized the Style Settings (and added a bunch as well, but this is a breaking change for your Style Settings so be careful when you update) as well as support for Hover Editor and more. 
* Here's [CSS for inline block references](https://gist.github.com/GitMurf/46c9ae78d6c3ce53d42d7832c7601271) that works for both NEW CM6 Live Preview and also Preview Mode for both CM5 (Legacy) and CM6 (New).

## Ancillary Code

* Here's an iOS-only [Shortcut for making a bare bones rich-text PDF](https://www.icloud.com/shortcuts/7fec6582678c48668583e78376598fab) from an Obsidian note

## Guides

* Here's a neat guide for [using custom checkboxes for a habit & mood tracker](https://github.com/corinnekaryiu/obsidian-habit-mood-tracker)
* This video presentation about [how to generate insights with maps of content](https://www.youtube.com/watch?v=UYVjzkjBeEA) got resurfaced. 
* Conrad Gessner was using slips of paper to rearrange and make connections in the 1500s. Here's [a book about it](https://mitpress.mit.edu/books/paper-machines). 
 * Here's a workflow for [managing professional writing in Obsidian](https://jamierubin.net/2022/04/05/practically-paperless-with-obsidian-episode-25-five-use-cases-for-managing-my-writing-in-obsidian/), from drafting manuscripts to managing writing projects, submissions, contracts, and seeing the big picture. It's [pretty similar to mine](https://www.youtube.com/watch?v=F4LE-nIzefM&list=PLGflcghBUIauy2We-93G3u8PQdx2DRSJi), with the addition of linking contract information to individual stories. 
 
## Showcases

* Here's a neat [taxonomic trees graph](https://twitter.com/rdmpage/status/1512177689028960264) inspired by this [tree of knowledge](https://kyletscheer.medium.com/on-creating-a-tree-of-knowledge-f099c1028bf6) writeup. 
* Here's a [personal knowledge management workflow from a computer scientist](https://sspaeti.com/blog/pkm-workflow-for-a-deeper-life/).
* Here's people sharing how they use Obsidian to [solve mysteries in fiction books](https://www.reddit.com/r/ObsidianMD/comments/tya4fh/im_using_obsidian_to_solve_an_agatha_christie/) and it's really neat!  
## Discussions

* Here's a lovely writeup from Sébastien Dubois about how their [25 years of personal knowledge management](https://dsebastien.net/blog/2022-04-03-25-years-of-personal-knowledge-management) led them to Obsidian, and the key lessons they learned along the way, with an [accompanying discussion on HackerNews](https://news.ycombinator.com/item?id=30903940).
* Here was an article that made the rounds this week about how [users are taking the internet back](https://www.protocol.com/newsletters/sourcecode/users-take-internet-back) and tools like Obsidian are one way they're doing it. There are some nice quotes from `@kepano`, the developer of Minimal. 
* Here are some tips for [copy and pasting from Obsidian to another program](https://www.reddit.com/r/ObsidianMD/comments/txnb4t/why_is_copy_pasting_from_obsidian_to_another_app/)
* There was a [Discord discussion](https://discord.com/channels/686053708261228577/744933215063638183/944902460533768222) about how to take notes using dataview, linked data/controlled vocabulary, and supercharged links. 
* Here's a [method for using kanban boards for course outlining](http://discordapp.com/channels/686053708261228577/722584061087842365/944512414534221844). 

## Ancillary Tools

* If you're a Windows user who is tired of hearing about how amazing Hazel is for automatically doing stuff with your files... I've been trying out [File Juggler](https://www.filejuggler.com/). I've been making local copies of articles I want to archive using the MarkDownload extension. File Juggler automatically moves the  `.md` files from my Downloads folder to my `Unaltered` folder Obsidian. It's not free, but it's a one-time purchase. 
* Here's an [alternative to Windows Explorer](https://www.gpsoft.com.au/) that got recommended. 

## Housekeeping

Periodically folks ask to send money to developers and moderators as a way to say thanks, but the developer or moderator is unable or unwilling to accept money directly. Today I stumbled across my note of charities that matter to `@argentum`, the moderator who handles publishing to the Hub, developed the MDNotes plugin for Zotero, and wrote and maintains Hotkeys++ and Natural Language Dates:

- [Coalition of Rainforest Nations](https://www.rainforestcoalition.org/)
- [Association for Women in Science - AWIS](https://www.awis.org/)
- [Give To Science Friday](https://www.sciencefriday.com/give-to-science-friday/)
- [Brain & Behavior Research Foundation](https://www.bbrfoundation.org/about)
- [The Planetary Society](https://www.planetary.org/)
- [Global Fund for Women](https://www.charitywatch.org/charities/global-fund-for-women)

If you're in a giving mood, consider sending some money their way in her name :) 