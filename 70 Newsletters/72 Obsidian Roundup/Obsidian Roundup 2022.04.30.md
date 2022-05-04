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
> - [Check Reddit](https://www.reddit.com/r/ObsidianMD/)
> - Some kind of pitch to the Iceberg if I don't have any other housekeeping notes. 

## In The Community

* Here's an open-source obsidian vault (via obsidian git and github) for maintaining notes on mathematical physics, physics and mathematics. It is [accepting contributions](https://github.com/Booodaness/Scientific-Notes). 
* An android developer is looking for ideas on [what mobile functionality the  community would like to have on hand](https://www.reddit.com/r/ObsidianMD/comments/uc9ijt/mobile_developer_looking_for_obsidian_mobile_app/) with the Obsidian app, more quickly? 

## Obsidian Updates

* Insider [v0.14.7](https://forum.obsidian.md/t/obsidian-release-v0-14-7-insider-build/36491) has a bunch of improvements for Obsidian Publish and Sync, including an improved setup guide for Sync, a new selector for light/dark mode on Publish, and more. 

## Plugin News

### New in Community Plugins

*These plugins went through code review and are now available in Obsidian's plugin list. For the full list, check out the [plugin stats page](https://obsidian-plugin-stats.vercel.app/new).*  

- [Omnisearch](https://github.com/scambier/obsidian-omnisearch) by `@scambier`  is the new and improved search. 
- [Calibre](https://github.com/caronchen/obsidian-calibre-plugin) by `@caronchen`  lets users access their calibre libraries and read books directly in Obsidian. 
- [Obsidian Columns](https://github.com/tnichols217/obsidian-columns) by `@tnichols217`  lets users create columns more easily.  
- [Drag-n-Drop for blocks](https://github.com/artem-barmin/obsidian-block-drag-n-drop) by `@artem-barmin`  Allows for moving/copying/creating embeds for blocks with drag-n-drop just like Logseq or Roam. 
- [Notion-Like Tables](https://github.com/trey-wallis/obsidian-notion-like-tables) by `@trey-wallis`  lets users create markdown tables using an interface similar to that found in Notion.

### Pending (as of Friday morning)

_Note: Not all new plugins are available in the community list yet, as they need to go through code review first. You can manually install plugins that aren't in the community list yet by using the [Beta Reviewer's Auto-update Tool](https://github.com/TfTHacker/obsidian42-brat). Note, though, that this is not as safe as waiting for them to go through code review._

- [Pandoc Reference List](https://github.com/mgmeyers/obsidian-pandoc-reference-list) by `@mgmeyers`  displays a formatted reference in the sidebar for each pandoc citekey present in the current document. 
- [Release Timeline](https://github.com/cakechaser/obsidian-release-timeline) by `@cakechaser`  requites Dataview, but lets users create "yes/no" style visuals like Wikipedia's release timelines. 
- [Filename Emoji Remover](https://github.com/YTolun/obsidian-filename-emoji-remover) by `@YTolun`  automatically removes emojis from filenames; this is really handy for sanitizing Readwise imports for Dropbox syncing. I filed [an issue](https://github.com/YTolun/obsidian-filename-emoji-remover/issues/1) suggesting it be expanded out for other filename sanitazation 👀 
- [Paste image Png to Jpeg](https://github.com/musug/obsidian-paste-png-to-jpeg) by `@musug`  compresses and renames screenshots when you paste them into Obsidian. 
- [Folder Index](https://github.com/turulix/obsidian-folder-index) by `@turulix`  will automatically generate a table of contents for the current folder. 
- [AutoMOC](https://github.com/dalcantara7/obsidian-auto-moc) by `@dalcantara7`  looks for missing linked mentions to the current note and imports them into the current note. 

### Updates

 _If you want a comprehensive list of what plugins updated this week, check out this [plugin updates index](https://obsidian-plugin-stats.vercel.app/updates) by Ganessh Kumar._

* [Collapse All v1.5.1](https://github.com/OfficerHalf/obsidian-collapse-all/releases/tag/1.5.1) collapses attachment folders by default, and adds some new commands to the right click menu. 
* [Task Collector 0.7.8](https://github.com/ebullient/obsidian-task-collector) now allows users to mark tasks in callouts and preserve strict line-ending spaces. 
* [Zotero Desktop Connector v2.0.0](https://github.com/mgmeyers/obsidian-zotero-desktop-connector/) simplifies import templates and [has new documentation](https://github.com/mgmeyers/obsidian-zotero-desktop-connector/blob/main/docs/Templating.md#how-do-i-prevent-sections-of-my-templates-from-being-overwritten). 
* [Code Editor Shortcuts v1.8.0](https://github.com/timhor/obsidian-editor-shortcuts/releases/tag/1.8.0) now allows users to select all (or just next) occurrences of the current selection. 
* [Advanced Slides 1.9.0](https://github.com/MSzturc/obsidian-advanced-slides) now has [template support](https://mszturc.github.io/obsidian-advanced-slides/templates/) and improved documentation. 
* The [JSON/CSV importer](https://github.com/farling42/obsidian-import-json) now has support for handlebars-helpers, select more than one source data file, and create note names according to JSON fields. 
* The [Snipd Podcast Player Integration](https://forum.obsidian.md/t/snipd-integration-podcast-highlights-with-transcript-notes-summary-metadata/26499/8) now allows users to listen to exported highlights directly from Obsidian, since all exported snips will now also include an embedded player.
* [Hover Editor](https://github.com/nothingislost/obsidian-hover-editor/releases) added a new setting to enable triggering Hover Editor when hovering over rendered embeds

### Betas

_Note: these plugins have not yet been submitted for code review, and are being made available primarily for testing purposes._

* [Calibre Importer](https://github.com/joethei/obsidian-calibre) lets you read your Calibre books directly in Obsidian _and_ allows you to import your book metadata and highlights from Calibre.

### For Developers

* Theme developers please check out this proposal for [creating an easier way to keep your information up to date in the community hub](https://github.com/obsidian-community/obsidian-hub/blob/main/00%20-%20Contribute%20to%20the%20Obsidian%20Hub/03%20Contributor%20Notes/03.02%20Design%20Decisions/hub.yaml%20proposal%20for%20themes.md). 

## Feature Requests

* [Visually distinguish stared notes in graph view](https://forum.obsidian.md/t/have-starred-notes-be-highlighted-on-the-graph/36601). 
* [AI driven autocomplete a la the gmail editor](https://www.reddit.com/r/ObsidianMD/comments/udzumy/software_that_can_be_used_in_obsidian_for_text/). 

## Appearance

* [AbsoluteGruv](https://github.com/kkYrusobad/AbsoluteGruv) by `@kkYrusobad`  
* Shimmering Focus differentiates between link types more clearly, prettier buttons, and got a bunch of other [new features](https://chrisgrieser.github.io/shimmering-focus/). 
* [Prism v2.0.0](https://github.com/damiankorcz/Prism-Theme) has 8 new color schemes, native styling for callouts, and other improvements but you _must_ install style settings (and restart) for it to work. 

## Guides

* Here's a [workflow for connecting a digital notebook with an analog one](https://blog.ulysses.app/ralph-caspers/), [explained and expanded on](https://discord.com/channels/686053708261228577/710585052769157141/969147759896711238) in Discord. 
* Here's a nice quick video guide on using [Obsidian for Dungeons & Dragons](https://www.youtube.com/watch?v=E-INzBocfSg), along with the [discussion on Reddit](https://www.reddit.com/r/ObsidianMD/comments/uckc6j/made_a_short_video_about_using_obsidian_notes_to/). 
* Here's a new guide for [syncing Readwise exports to Obsidian](https://www.youtube.com/watch?v=i-nlLOXr0Lg). 
* Here's a [task management system](https://forum.obsidian.md/t/my-task-management-system/36198/3) writeup. 
* Here's a new way to use [Alfred Pandoc Suite with Obsidian](https://forum.obsidian.md/t/use-alfred-pandoc-suite-with-obsidian-to-export-pdf-with-citation-and-bibliography/36702) to export PDF with citation and bibliographies. 
## Discussions

* Here's some tips for using [Dataview to make Eisenhower matricies](https://www.reddit.com/r/ObsidianMD/comments/udtb2s/simple_solution_to_integrate_eisenhower_matrix/). 
* Here's [6 months of PhD work as a timelapsed graph](https://www.reddit.com/r/ObsidianMD/comments/uds6cy/6_months_of_phd_work_as_a_timelapse_of_my_vaults/). There's also a nice associated discussion on Reddit. 
* Several people commented on an article about [how someone used Obsidian for their PhD](https://www.reddit.com/r/ObsidianMD/comments/ua6v76/i_wrote_a_short_article_about_how_i_use_obsidian/). 
* Here's a discussion of different [daily notes workflows for academics](https://www.reddit.com/r/ObsidianMD/comments/ud2jz9/please_share_daily_notes_workflow_for_academics/). 
* Here's a discussion [comparing flashcard plugin options](https://www.reddit.com/r/ObsidianMD/comments/ucrkt7/whats_the_best_obsidian_flashcard_plugin/). 
* Here's a nice discussion about [how people use Obsidian mobile](https://www.reddit.com/r/ObsidianMD/comments/ubwsfs/for_those_of_you_that_use_obsidian_on_your_phone/). 
* This one is a nice compilation of [clever tricks for using Obsidian](https://www.reddit.com/r/ObsidianMD/comments/uaxzhf/what_clever_obsidian_tricks_have_you_found/). 
* Here's a nice writeup and accompanying discussion about how to [keep things simple with Obsidian](https://www.reddit.com/r/ObsidianMD/comments/u9uq8k/does_obsidian_seem_too_complicated_or/) so it doesn't feel too complicated. 
* Here's a nice discussion with advice about [how to create a maintainable second brain](https://forum.obsidian.md/t/a-maintainable-second-braind-for-someone-with-adhd/36106). 

## Ancillary Tools

- The social highlighting tool [Glasp](https://forum.obsidian.md/t/export-web-articles-into-obsidian/36679) now supports [one-click exports to Obsidian](https://forum.obsidian.md/t/export-web-articles-into-obsidian/36679). 