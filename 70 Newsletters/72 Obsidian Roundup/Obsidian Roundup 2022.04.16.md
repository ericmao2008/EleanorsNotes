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

## Obsidian Updates

The new public release used Electron 18; if you noticed something weird with your PDFs, [get the Electron 17 based installer](https://forum.obsidian.md/t/obsidian-release-v0-14-5/35094). 

Also, as of [Insider 0.14.6](https://forum.obsidian.md/t/obsidian-release-v0-14-6-insider-build/35640), users can now add folders to an ignore filter. Files matched by this filter will be down-ranked when using Quick Switcher and link suggestions, and will be excluded in search results and graph view. 

## Plugin News

### Pending (as of Friday morning)

_Note: Not all new plugins are available in the community list yet, as they need to go through code review first. You can manually install plugins that aren't in the community list yet by using the [Beta Reviewer's Auto-update Tool](https://github.com/TfTHacker/obsidian42-brat). Note, though, that this is not as safe as waiting for them to go through code review._

- [Drag-n-Drop for blocks](https://github.com/artem-barmin/obsidian-block-drag-n-drop) by `@artem-barmin`  allows for the moving/copying/and creation embeds for blocks with drag-n-drop just like Logseq or Roam. 
- [Book Search](https://github.com/anpigon/obsidian-book-search-plugin) by `@anpigon`  automatically creates notes by searching for books by book title, author, publisher or ISBN (10 or 13). It uses the Google Books API to get the information.
- [Obsidian Ghost Publish](https://github.com/jaynguyens/obsidian-ghost-publish) by `@jaynguyens`  allows for single click publishing to the Ghost publishing platform. 
- [Snippet Downloader](https://github.com/Mara-Li/obsidian-snippet-downloader) by `@Mara-Li`  is basically a snippet manager for people who have a lot of snippets they downloaded from gists and repositories. 
- [Link Keeper](https://github.com/luhaifeng666/obsidian-link-keeper) by `@luhaifeng666`  is intended to help manage frequently used links.  
- [Obsidian jTab](https://github.com/davfive/obsidian-jtab) by `@davfive`  adds the ability to show guitar chords and tabs directly in your notes using jTab. 
- [Notion-Like Tables](https://github.com/trey-wallis/obsidian-notion-like-tables) by `@trey-wallis`  lets you create markdown tables using an interface similar to that found in Notion.so. 
- [Template Enabled Day Planner](https://github.com/amykhar/obsidian-day-planner-with-templates) by `@amykhar`  is for day planning and managing pomodoro timers from a task list in a Markdown note.
- [Typing speed](https://github.com/Supercip971/obsidian-typing-speed) by `@Supercip971`  will show the current typing speed in the status bar 
- [Paste image rename](https://github.com/reorx/obsidian-paste-image-rename) by `@reorx`  supports name patterns and auto renaming.
- [KoreanBook Info Plugin](https://github.com/kmsk99/kr-book-info-plugin) by `@kmsk99`  crawls the  online book retailer Yes24 to get book information. 

### Updates

* [Various Complements plugin v5.11.0](https://github.com/tadashi-aikawa/obsidian-various-complements-plugin/releases/tag/5.11.0) got some improvements to reduce the likelihood of conflicts with other plugins. 
* [Another Quick Switcher plugin v4.8.0](https://github.com/tadashi-aikawa/obsidian-another-quick-switcher/releases/tag/4.8.0) got some new hotkeys
* [Full Calendar](https://github.com/davish/obsidian-full-calendar) now supports one-way sync with private Apple Calendars, along with any calendar that uses the CalDAV protocol over HTTP basic authentication.
* [QuickAdd v0.5.4](https://github.com/chhoumann/quickadd) added support for aliases in the file suggester.
* [Custom Frames](https://github.com/Ellpeck/ObsidianCustomFrames#%EF%B8%8F-markdown-mode) now supports displaying custom frames in your markdown documents, i.e. embedding a calendar in your daily notes. You can also add a ribbon icon for any frame you want, and display a frame in the center editor.
* The [typewriter scroll](https://github.com/deathau/cm-typewriter-scroll-obsidian/releases/tag/0.2.2) plugin can now be toggled on/off without having to reset obsidian. You can also set the scroll offset now. 

### Betas

_Note: these plugins have not yet been submitted for code review, and are being made available primarily for testing purposes._

* [Omnisearch](https://github.com/scambier/obsidian-omnisearch) is developing into an improved search method for Obsidian. It weights different parts of the file (name, title, body) differently, reacts intelligently to typos, and has better fuzzy search. 
* [Periodic Notes 1.0 Beta](https://github.com/liamcain/obsidian-periodic-notes) supports _multiple_ daily notes per day, and frontmatter support so you can name your files whatever you want. 
* [mkdocs publisher](https://github.com/Mara-Li/obsidian-mkdocs-publisher) — [Obs2mk](https://github.com/Mara-Li/mkdocs_obsidian_publish) now has better support for Github Actions, and a plugin! There are [more details in Discord](https://discord.com/channels/686053708261228577/855181471643861002/963373533688397875)

 ## Feature Requests

* It really would be nice if we could [search pdfs from inside of Obsidian](https://forum.obsidian.md/t/search-a-pdf/15079). 
* Here are some suggested [graph node size customizability](https://forum.obsidian.md/t/allow-to-configure-how-node-size-is-calculated/4247) options. In a similar vein, it would be nice if [folders had any impact on the graph view whatsoever](https://forum.obsidian.md/t/cluster-notes-in-graph-view/2493/2). 

## Appearance

* [AbsoluteGruv](https://github.com/kkYrusobad/AbsoluteGruv) by `@kkYrusobad`  should be coming to the community list soon. 
* [Shimmering Focus](https://chrisgrieser.github.io/shimmering-focus/) hides floating metadata blocks & YAML frontmatter, tho this can be disabled with Style Settings. Footnotes in Reading mode do not affect line height anymore, and there are now hue sliders in Style settings, which should make customizing colors easier. 
* [Blue Topaz](https://github.com/whyt-byte/Blue-Topaz_Obsidian-css) supports multiple calendars, and improved callout types. 
* [Willemstad X v0.4.0 Nyhavn](https://github.com/tingmelvin/willemstad-x/releases/tag/v0.4.0) got a bunch of breaking changes involving more customizations, particularly for custom readable line lengths. 
* Here's a guide on how to get a [beautiful homepage](https://github.com/Rainbell129/Obsidian-Homepage). 

## Guides

* Here's a nice guide for using Obsidian while [working with CSS, markdown and Javascript on an iPad](https://tfthacker.medium.com/customizing-obsidian-on-your-ipad-8b71019a276c).
* Here's an updated [academic workflow using Obsidian and Zotero](https://medium.com/@alexandraphelan/an-academic-workflow-zotero-obsidian-56bf918d51ab) — specifically the new Zotero Desktop Connector plugin. 
* Here's a "starter kit" for [automated weekly reviews](https://github.com/Pamela-Wang/Automated-Obsidian-Weekly-Review) which uses Dataview inline fields to rollup into weekly logs, and also the tracker plugin as a habit tracker.  It comes with a handy [video](https://youtu.be/tUWjyzvljfs). 
* Here's a guide on Discord about how to use [Citavi for generating directories of notes by publication](https://discord.com/channels/686053708261228577/722584061087842365/964112036080525312).
* Here's a hack to [force install hover editor on a tablet](https://twitter.com/TfTHacker/status/1510329797003644940). 
* Here's how to [manage blog writing](https://jamierubin.net/2022/04/12/practically-paperless-with-obsidian-episode-26-use-case-managing-my-blog-writing-in-obsidian/) using Obsidian. 
* The Hub has a new guide for [automatic plugin testing](https://publish.obsidian.md/hub/04+-+Guides%2C+Workflows%2C+%26+Courses/for+Plugin+Developers+to+Automate+Tests), and added new ways to [use Zettelkasten for creative writing](https://publish.obsidian.md/hub/04+-+Guides%2C+Workflows%2C+%26+Courses/for+Creative+Writing).

## Discussions

* Here's a big discussion (189 replies!) on Reddit about [people's biggest pain points](https://www.reddit.com/r/ObsidianMD/comments/u2lvho/what_are_some_of_your_current_frustrations_with/) (and, in some cases, which plugins could help solve them :D)
* Here's a discussion on Twitter about [how to indicate whether a claim is weak or strong](https://twitter.com/syncretizm/status/1514967364827185159). 
* Over on Twitter, I shared a quick example of a situation for why I prefer to [leave quotes in my source notes](https://twitter.com/EleanorKonik/status/1514619474007113739) instead of spinning them out into my atomic notes with stuff like the note composer plugin (or [this alternate Zettelizerscript](http://discordapp.com/channels/686053708261228577/710585052769157141/960549102247116840)). A couple of other people shared how they prefer to do it. 
* Here's a discussion about [various methods to encrypt a vault](https://www.reddit.com/r/ObsidianMD/comments/u3nsf6/passwordlock_vaults/).
* Reddit has some good advice for people [taking lecture notes on new topics](https://www.reddit.com/r/ObsidianMD/comments/u2uoj7/what_the_hell_do_we_do_about_lectures_newby_in/). 
* And for people [using Obsidian to manage engineering](https://www.reddit.com/r/ObsidianMD/comments/u0fdxf/does_anyone_use_obsidian_in_an_engineering/). 

## Showcases

* Here's a really neat [physics and math wiki](https://publish.obsidian.md/myquantumwell/Quantum+Mechanics/Unitary+transformations+in+quantum+mechanics). 

## Ancillary Tools

* The [Raycast Obsidian extension](https://www.raycast.com/marcjulian/obsidian) now has support for opening and creating daily notes, appending selected text to ntoes, prefixes for appended text, and more. 
* Here's how to [bulk pull DOIs for all your papers](https://twitter.com/ymshulman/status/1482521841512157187) in Zotero, even if they don't have DOIs yet. 
* Here's a new alternative to [Obsidian publish](https://www.reddit.com/r/ObsidianMD/comments/u3irg6/a_free_simple_good_looking_alternative_to/). It has a pretty nifty graph view and nicely slugified URLs. 

## Housekeeping

Now that I'm writing more essays, I decided it was time to overhaul the Roundup's [landing page](https://www.obsidianroundup.org/). There's also now a button at the bottom to let you get into dark mode; just click the moon to get into dark mode, or the sun to get into light mode. It's to the right of the RSS button :) 

Also, I got a couple of reports of something going wrong with my email automation (edge case McGee strikes again!) — if you got duplicate emails from me I'm so sorry and am working on getting it resolved :( 