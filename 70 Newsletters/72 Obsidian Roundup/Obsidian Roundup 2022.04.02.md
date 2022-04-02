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

* Here's a really lovely [thread for sharing appreciation for the developers of Obsidian](https://forum.obsidian.md/t/lets-show-erica-and-shida-some-love/34704). 
* Nick Milo and I caught up live; you can watch the recording of us sharing updates to our workflows over on Youtube. Mostly we talked about [quick notes & cognitive scaffolding](https://www.youtube.com/watch?v=8IL0wFUT6XQ). 
* This wasn't an April Fool's joke, but as far as bugs go, it was [oddly charming](https://www.reddit.com/r/ObsidianMD/comments/tpxk45/obsidian_annoying_sound/). 
* Here's the [April Fool's joke](https://obsidian.md/cloud). (And last April's [quiz](https://obsidian.md/quiz), which is now a lot harder than it used to be). 

### Hub

_The Obsidian Hub is a community knowledge base designed to help organize information about the Obsidian ecosystem. It's an excellent companion to this Roundup, which tends to be very chronological in nature. Here are some of the [recent updates](https://github.com/obsidian-community/obsidian-hub/pulls?q=is%3Apr+is%3Amerged+sort%3Aupdated-desc+-label%3A%22scripted+update%22+-label%3A%22hub+tools+%26+scripts%22+%3E+)_: 

- The last 3 months or so of [the Obsidian Roundup](https://publish.obsidian.md/hub/01+-+Community/Obsidian+Roundup/%F0%9F%97%82%EF%B8%8F+Obsidian+Roundup) have been indexed in the Hub thanks to the herculean efforts of Luke & Claire. 
- Here's a list of [plugins that could use help from the community](https://publish.obsidian.md/hub/01+-+Community/Contributing+to+the+Community/Plugins+seeking+help). 
- There's a new index of [plugins useful for collaboration](https://publish.obsidian.md/hub/02+-+Community+Expansions/02.01+Plugins+by+Category/Plugins+for+collaboration). 

## Obsidian Updates

Obsidian now offers [40% off education and non-profit discounts](https://help.obsidian.md/Student+and+non-profit+discount) for Obsidian Sync and Publish. 

From [Insider 0.14.3](https://forum.obsidian.md/t/obsidian-release-v0-14-3-insider-build/34806) & [0.14.4](https://forum.obsidian.md/t/obsidian-release-v0-14-4-insider-build/35026)

- You can now move, rename or locate your vaults directly from the vault switcher.
- The local help vault has been replaced with a sandbox vault; there's also a new in-app help page with links to the online help docs, Discord, forum.
- You can now set the font for the interface and the editor directly under appearance settings. Note that some themes may override this font setting.
-  Vim mode up/down now goes into rendered code blocks, embeds, callouts, or tables in Live Preview instead of skipping them.
- Pasting and dropping images or media files that are already located in the vault will now link to it directly instead of duplicating the file.
- Obsidian Sync now has a fully customizable sync folder exclusion system. This allows you to add exclusions to folders even if they don’t exist locally.
- Toggle bold/italics will now smartly skip over the closing markers when at the end of the block, instead of adding more marker symbols.

## Plugin News

### Pending (as of Friday morning)

_Note: Not all new plugins are available in the community list yet, as they need to go through code review first. You can manually install plugins that aren't in the community list yet by using the [Beta Reviewer's Auto-update Tool](https://github.com/TfTHacker/obsidian42-brat). Note, though, that this is not as safe as waiting for them to go through code review._

- [Control Characters](https://github.com/joethei/obsidian-control-characters) by `@joethei`  lets users see control/non-printing characters in edit mode. 
- [Text Toolbar](https://github.com/farux/obsidian-text-toolbar) by `@farux`  is customizable toolbar that allows CSS snippets, markdowns, and built-in macros to be applied to selected text. 
- [File Explorer Toolbar](https://github.com/oslog/obsidian-file-explorer-toolbar) by `@oslog`   displays currently open files in the toolbar of file explorer. 
- [Chat View](https://github.com/adifyr/obsidian-chat-view) by `@adifyr`  can create an elegant Chat UI in Obsidian markdown files. 

### Updates

 _If you want a comprehensive list of what plugins updated this week, check out this [plugin updates index](https://obsidian-plugin-stats.vercel.app/updates) by Ganessh Kumar._

- [Zotero Desktop Connector](https://github.com/mgmeyers/obsidian-zotero-desktop-connector) by `@mgmeyers`  is now available in the Community Plugins list and got some documentation. It supports specific citation and bibliography styles, and lets you create templates for importing notes directly from Zotero desktop. 
* [File Tree Alternative](https://github.com/ozntel/file-tree-alternative) 2.0 allows for a lot more dragging and dropping and collapsing. 
* [Another Quick Switcher plugin v4.5.0](https://github.com/tadashi-aikawa/obsidian-another-quick-switcher/releases/tag/4.5.0) enabled searching by tags even if queries don't start with `#`.
* [Customizable Page Header and Title Bar](https://github.com/kometenstaub/customizable-page-header-buttons) added support for the backward/forward count display of pane relief which you can activate in the settings.
* [Obsidian Git](https://github.com/denolehov/obsidian-git/pull/165) reworked the diff view system and added automatic refreshing of Source Control view. 

### Betas

_Note: these plugins have not yet been submitted for code review, and are being made available primarily for testing purposes._

* [List Modified](https://github.com/franciskafieh/obsidian-list-modified/releases/tag/0.0.1) is a neat new plugin where, when you modify a file, it will automatically be linked to your daily note. You can create tag blacklists that prevent notes with certain tags from being linked to.

### For Developers

* As of [Insider 0.14.3](https://forum.obsidian.md/t/obsidian-release-v0-14-3-insider-build/34806), callouts have metadata, DOMPurify, Turndown, Mermaid, PIXI.js, and Prism.js got updated, and there were a bunch of URI updates, including an optional `append` flag that should make things easier for developing shortcuts and such. Also, CSS variables related to fonts have been renamed.
* [Admonitions v9.0.0](https://github.com/valentine195/obsidian-admonition/releases/tag/9.0.0) got a breaking change that will impact styling; it now mimics the structure of callouts. 

## Feature Requests

* [Keyboard navigation for settings search](https://forum.obsidian.md/t/keyboard-navigation-and-searching-in-settings/15556) 
* A [toggle to open all links in new panes](https://forum.obsidian.md/t/toggle-to-open-all-links-in-new-pane/29484/9). 

## Appearance

* Here's a snippet to get [Craft-style tabs](https://gist.github.com/kepano/7fc1cd9433b5506ce45b44cfa3734fa0) in the Minimal theme. 
* [Dracula + LYT](https://github.com/xRyul/ObsidianMD_Dracula_x_LYT) is a blend of LYT Mode and Dracula color schemes. 
* [Minimal](https://github.com/kepano/obsidian-minimal/releases/tag/5.1.9) is now compatible with the new and improved Hover Editor plugin and several others. 
* [Willemstad X v0.3.0 Bryggen](https://github.com/tingmelvin/willemstad-x/releases/tag/v0.3.0) reworked the Style Settings menus and added a bunch of stuff for tables, admonitions, and callouts. 
* [Primary](https://github.com/ceciliamay/obsidianmd-theme-primary/releases/tag/v.1.4.4) is now more customizable. 

## Guides

* Here's an awesomely comprehensive guide for [how to use Obsidian sync](https://curtismchale.ca/2022/03/30/everything-you-need-to-know-about-obsidian-sync/) via Curtis McHale
* Here's a really nice step-by-step guide for [How to Turn Your Notes into a Database with Obsidian and Dataview](https://www.makeuseof.com/obsidian-dataview-notes-guide/) aimed at beginners. 
* Here's a [deep dive on DataviewJS](https://www.youtube.com/watch?v=d8plJSJYqVw) that got resurfaced during discussion. 
* Here's a [workaround](https://medium.com/@tfthacker/using-readwises-highlight-id-as-a-single-source-of-truth-in-obsidian-b1de98a8b87c) you can use if you're experiencing duplicate content with Readwise; here's [more explanation](http://discordapp.com/channels/686053708261228577/694233507500916796/957381064425369610) in Discord. 
* [AP Productivity Cohort 4](https://courses.rjnestor.com/p/ap-productivity) is starting soon, and they've added an Obsidian-focused section. I'm told it's particularly good for time-management type things. 
* Here's how to use [Quartz as a free Publish alternative](https://youtu.be/ITiiuBNVue0)

## Discussions

* Reddit had a nice discussion of putting [meeting notes in your daily note](https://www.reddit.com/r/ObsidianMD/comments/truxbn/meeting_minutes_in_daily_note/). 
* Here was a discussion about [categories of notes](https://discord.com/channels/686053708261228577/710585052769157141/958396973348696114) in Discord. 
* Here's a Discord discussion about [using Obsidian on an iPad without an external keyboard](http://discordapp.com/channels/686053708261228577/864046194195431425/959293102424727573). 
* Here's a cool trick for college notetaking: Google map can't identify [individual lecture halls as locations for your notes](http://discordapp.com/channels/686053708261228577/710585052769157141/958623521846722590)... but Leaflet can. 
* Here's a discussion about what plugins can support the [programmable notes](https://www.reddit.com/r/ObsidianMD/comments/tpfgi1/read_an_article_on_programmable_notes_are_there/) workflow from Maggie Appleton. 
* Here's some tips on [how to manage genealogies in Obsidian](https://www.reddit.com/r/ObsidianMD/comments/tr1c31/tips_for_genealogy_and_biography_work_using/). 

## Ancillary Tools

* [Google Docs now supports markdown](https://workspaceupdates.googleblog.com/2022/03/compose-with-markdown-in-google-docs-on.html). 

## Housekeeping

Next week, I'm going to be increasing the price of the Iceberg from $2/mo to $3/mo. If you've ever been curious about what my vault looks like when it's actually in Obsidian, instead of just poking around the public published versions, now's a good time. The `.zip` version ships with my stories and worldbuilding notes, which just got a big overhaul to be a lot more clearer and comprehensive. 