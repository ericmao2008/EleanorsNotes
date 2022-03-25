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

* Nick Milo is hosting me for a livestream event tomorrow 2022-03-27 at 2pm EST. The topic will be [quick notes & cognitive scaffolding](https://www.youtube.com/watch?v=8IL0wFUT6XQ); watch live as Nick and I catch each other up on what's new with our workflows. 
* There will be a community talk about [easy automated testing for plugins](https://discord.com/events/686053708261228577/955086222261383238) on Saturday, April 9 at 9:30 EST. 
* Some of us are trying to crowdsource information about the current state of pdf/zotero/citations plugins and workflows. If you do anything with Obsidian and those things, please [check out this thread](https://forum.obsidian.md/t/pdf-zotero-obsidian-current-state-and-collaboration-for-the-one-plugin/34372) and contribute your thoughts & insights. 

### Hub

_The Obsidian Hub is a community knowledge base designed to help organize information about the Obsidian ecosystem. It's an excellent companion to this Roundup, which tends to be very chronological in nature. Here are some of the [recent updates](https://github.com/obsidian-community/obsidian-hub/pulls?q=is%3Apr+is%3Amerged+sort%3Aupdated-desc+-label%3A%22scripted+update%22+-label%3A%22hub+tools+%26+scripts%22+%3E+)_

## Obsidian Updates

Obsidian Mobile Insider v1.2.0 has feature parity with Core v.0.14.2 (the new callouts). The iOS Share extension is also available - you can now share text, links, images and attachments to the Obsidian app and have it inserted into the note. (Android already had this functionality for a while).

## Plugin News

### New in Community Plugins

*These plugins went through code review and are now available in Obsidian's plugin list.* For the full list, check out the [plugin stats page](https://obsidian-plugin-stats.vercel.app/new). 

- [Hover Editor](https://github.com/nothingislost/obsidian-hover-editor) transforms the Page Preview hover popover into a fully working editor instance. The Hover Editor title bar has window controls such as minimize, maximize, and close. They can be split and linked just like normal workspace panes, which includes linking a hover editor pane to a normal workspace pane. You can also drag native Obsidian leaves into a Hover Editor.
- [Custom Frames](https://github.com/Ellpeck/ObsidianCustomFrames) by `@Ellpeck`  turns web apps into panes using iframes with custom styling. It comes with presets for Google Keep, so you can embed your shared shopping list into Obsidian now. 
- [Buttondown](https://github.com/caro401/obsidian-buttondown) by `@caro401`  lets users send notes to buttondown.email accounts as email drafts. 
- [Quiet Outline](https://github.com/guopenghui/obsidian-quiet-outline) by `@guopenghui`  makes the outline more powerful, including no-auto-expand, rendering heading as markdown, and search support. 

### Pending (as of Friday morning)

_Note: Not all new plugins are available in the community list yet, as they need to go through code review first. You can manually install plugins that aren't in the community list yet by using the [Beta Reviewer's Auto-update Tool](https://github.com/TfTHacker/obsidian42-brat). Note, though, that this is not as safe as waiting for them to go through code review._

- [Simple Mention](https://github.com/der-tobi/obsidian-simple-mention) by `@der-tobi`  
    - Get highlighted mentions and mention suggestions. Find all occurrences of a mention 
- [Smort](https://github.com/SmortApp/obsidian-smort) by `@getsmort`  
    - Add Smort.io articles to Obsidian. Smort.io lets you easily edit, annotate and share articles. 

### Updates

 _If you want a comprehensive list of what plugins updated this week, check out this [plugin updates index](https://obsidian-plugin-stats.vercel.app/updates) by Ganessh Kumar._

* [Version history diff](https://github.com/kometenstaub/obsidian-version-history-diff) now allows you to view git diffs in addition to file recovery plugin & sync versions. 
* [Topic Linking](https://github.com/liammagee/obsidian-topic-linking/releases) (which extracts the contents of pdfs and web links for easier indexing and then groups them into topics based on natural language analysis) added support for extraction of highlights and comments. 
* [Settings Search](https://github.com/valentine195/obsidian-settings-search/releases/tag/1.2.0) now works on mobile. 
- [Icon Folder](https://github.com/FlorianWoelki/obsidian-icon-folder) added functionality for adding custom icon packs and icons, i.e. font-awesome. 
* [Code Editor Shortcuts](https://github.com/timhor/obsidian-editor-shortcuts/releases/tag/1.6.0) v1.6.0 added `delete to end of line`, `move cursor left/right` and `go to previous/next line`. 
* [remotely-save](https://github.com/remotely-save/remotely-save) now allows syncing `_` files, and the `.obsidian` special folder. It also added Chinese support. 
* [Smarter Markdown Hotkeys](https://obsidian.md/plugins?id=obsidian-smarter-md-hotkeys) got some new features, including stuff like `Smarter Delete File` which deletes the current file and goes back to the last note instead of leaving an empty pane behind.
* The [map of content](https://github.com/Robin-Haupt-1/Obsidian-Map-of-Content/releases) plugin now has a command palette command for opening the map view. 

### Betas

_Note: these plugins have not yet been submitted for code review, and are being made available primarily for testing purposes._

* [Mindful Obsidian](https://github.com/Panossa/mindful-obsidian/releases) makes your "Delete" buttons red. More broadly, adds the ability to style context menu elements via CSS. Either via title or icon value. 

### Under The Radar

### For Developers

## Feature Requests

## Appearance

### Plugins

* Version 4.0.0 of [Customizable Page Header](https://obsidian.md/plugins?id=customizable-page-header-buttons) added support for lucide icons and removed feather icons.

### Themes

* [Primary](https://github.com/ceciliamay/obsidianmd-theme-primary) added styling for hover editor boxes & callouts. It also changed the styling for `data-task` checkboxes to align with the emerging standards, i.e. `[v]` is now `[b]` for bookmarks, `[p]` is now `[c]` for thumbs-down (con), etc. There are [more details in the release notes](https://github.com/ceciliamay/obsidianmd-theme-primary/releases/tag/v.1.4.0). 
- There's a new theme: [Aqua](https://github.com/sahilpatel09/Aqua-obsidian) by `@sahilpatel09`  
* v0.2.7 of [the Willemstad theme](https://github.com/tingmelvin/willemstad-x/releases/tag/v0.2.7) added kanban and kanban-no-title callout classes in-note so that (pseudo-)kanbans can work on Obsidian Publish. The syntax should work if you port the markdown content over from the Kanban plugin. This is in addition to table, infobox, aside, aside-no-title callouts. Here's the code [as css snippets](https://github.com/tingmelvin/willemstad-x/blob/main/snippet.css). 

### Snippets

* Here's a snippet to get [Craft-style tabs](https://gist.github.com/kepano/7fc1cd9433b5506ce45b44cfa3734fa0) in the Minimal theme. 
* Here's some CSS to [style individual callout boxes](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Guide/Callouts.md) without relying on a theme. 

## Ancillary Code

* The [mkdocs plugin](https://github.com/Mara-Li/mkdocs_embed_file_plugins) (an alternative method for publishing your files) now supports wikilinks and image wikilinks. 
* Here's a method to [promote and demote heading levels](https://forum.obsidian.md/t/promote-demote-all-selected-headers/25799/8?u=eleanorkonik). 
## Guides

* Here's a new guide for [planning and writing fiction in Obsidian](https://write.as/vanessaglau/how-i-plan-and-write-fiction-in-obsidian) via Vanessa Glau. 
* Here's a nice how-to video for [implementing Zettelkasten in Obsidian by processing Readwise notes](https://www.youtube.com/watch?v=Rw1L5sxlnuU). 

## Discussions

* I wrote a [quick thread](https://typefully.com/EleanorKonik/HhUXuqG) about why I chose Obsidian as my Worldbuilding app. 
* Obsidian makes many appearances in this discussion from Hacker News about [plaintext productivity](https://news.ycombinator.com/item?id=30745524), which is a [productivity system](https://plaintext-productivity.net/) designed for Windows. 
* Here was another discussion about [how to use Obsidian for programming notes](https://www.reddit.com/r/ObsidianMD/comments/ti0esx/does_anyone_use_obsidian_for_their_programming/) with a focus on the Jupyter plugin. 
## Knowledge Management

## Ancillary Tools

* Here's a nice [list of annotation tools](https://beepb00p.xyz/annotating.html) that adds a lot of context and explanation and tips, by someone who has an _incredibly comprehensive_ website outlining workflows and processes for notetaking in plaintext. It's created by an `org-mode` person, but the information is broadly applicable. 

## Housekeeping
