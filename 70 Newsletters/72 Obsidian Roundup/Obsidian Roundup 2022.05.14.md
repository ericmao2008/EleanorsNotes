No> [!INFO] Creation Steps
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

The [Linking Your Thinking Conference](https://www.linkingyourthinking.com/conference) is a week of free workshops that "explores how to use linked notes in practical and powerful ways." It's hosted by Nick Milo, and runs from Mon, May 16 to Fri, May 20. Speakers include Ramses Oudt, David Sparks, Nicole van der Hoeven, Bianca Pereira & me.

I'll be speaking at the Linking Your Thinking Conference about `Synthesizing Research into Using Notes Without Plugins`. The talk will be May 17 at 11:00 AM PDT. Here's [a registration link](https://lu.ma/cv7d859j).  

## Obsidian Updates

The big update this week was [collaborative sync improvements](https://forum.obsidian.md/t/obsidian-release-v0-14-10-insider-build/37292), which are currently being tested by Insiders. You can now share your Obsidian Sync vaults with others. Collaborators must have an Obsidian Sync subscription, but joining a Sync vault will not count towards the 5 vault limit for collaborators.

## Plugin News

### New in Community Plugins

*These plugins went through code review and are now available in Obsidian's plugin list.* For the full list, check out the [plugin stats page](https://obsidian-plugin-stats.vercel.app/new). 

- [Obsidian Enhancing Export](https://github.com/mokeyish/obsidian-enhancing-export) by `@mokeyish`  is a new Pandoc plugin that allows to export to formats like Html, DOCX, ePub and PDF or Markdown(Hugo) etc. 
- [ePub Reader](https://github.com/caronchen/obsidian-epub-plugin) by `@caronchen` lets users open `.epub` files. 

### Pending (as of Friday morning)

_Note: Not all new plugins are available in the community list yet, as they need to go through code review first. You can manually install plugins that aren't in the community list yet by using the [Beta Reviewer's Auto-update Tool](https://github.com/TfTHacker/obsidian42-brat). Note, though, that this is not as safe as waiting for them to go through code review._

- [Date in metadata](https://github.com/salmund/obsidian-date-in-metadata) by `@salmund`  automatically inserts the date in YAML frontmatter on file creation. 
- [Nuke Orphans](https://github.com/sandorex/nuke-orphans-plugin) by `@sandorex`  deletes orphaned files and attachments. 
- [Weread Plugin](https://github.com/zhaohongxuan/obsidian-weread-plugin) by `@zhaohongxuan`  syncs Weread(微信读书) hightlights and annotations into your Obsidian Vault.
- [Upcoming](https://github.com/charliecm/obsidian-upcoming) by `@charliecm`  lets users open upcoming daily notes in their own panes. 
- [BBCode Convertor](https://github.com/salockhart/obsidian-bbcode) by `@salockhart`  can convert your markdown files to BBCode. 
- [YouTube Timestamp Notes](https://github.com/juliang22/ObsidianYoutubeTimestampNotes) by `@juliang22`  allows side-by-side notetaking with YouTube videos; it lets users annotate notes with timestamps to directly control the video and record where each note comes from. 
- [Local Quotes](https://github.com/ka1tzyu/local-quotes) by `@ka1tzyu`  is an interesting new take on spaced repetition that collects your quotes from all over the repository and embeds them.
- [Obsidian Functionplot](https://github.com/leonhma/obsidian-functionplot) by `@leonhma`  offers another method for displaying mathematical graphs.
- [Code Embed](https://github.com/Y-jiji/code-embed) by `@Y-jiji`  allows users to embed files (like `xx.c` `xx.hs` `xx.cpp`)  into  notes just like `.pdf` files; this is useful for taking competitive-coding notes (on ICPC, Codeforces, ... etc.). 
- [User Plugins](https://github.com/mnowotnik/obsidian-user-plugins) by `@mnowotnik`  allows users to use `.js` files or snippets to code quick and dirty plugins. 

### Updates

 _If you want a comprehensive list of what plugins updated this week, check out this [plugin updates index](https://obsidian-plugin-stats.vercel.app/updates) by Ganessh Kumar._

* [Omnisearch 1.2.1](https://github.com/scambier/obsidian-omnisearch) added support for "quoted expressions" and -exclusions.
* [Another Quick Switcher plugin v4.10.0](https://github.com/tadashi-aikawa/obsidian-another-quick-switcher/releases/tag/4.10.0) & v4.11.0 both improved support for headers. 
* [Advanced Slides 1.10.0](https://github.com/MSzturc/obsidian-advanced-slides)  added support for webp images and autocomplete suggestions. 1.11.0 added support for Obsidian charts, embedding slides into Obsidian notes, syntax suggestions, and more documentation. 
* [Various Complements plugin v6.1.0](https://github.com/tadashi-aikawa/obsidian-various-complements-plugin/releases/tag/6.1.0) added support for Custom dictionary files in JSON format. 
* The [Database plugin](https://github.com/tomaszkiewicz/obsidian-database-plugin/releases/tag/1.0.3) (like Dataview, but editable) added support for a dropdown control with multiple values, improved color handling, added checkbox support and clickable link fields (also with possibility for multiple values).
* [Pandoc Reference List](https://github.com/mgmeyers/obsidian-pandoc-reference-list) will now indicate when a citekey does not exist in your bibliography file
* [Enhanced Copy Note](https://github.com/kzhovn/copy-command-obsidian) will let users duplicate a selected folder and all its contents. 

### For Developers

* [v0.8.0 of the Pocket plugin](https://github.com/nybbles/obsidian-pocket) is out, and the [developer is looking for a new maintainer to take over](https://twitter.com/nimalan/status/1524802144796172290). 

## Feature Requests

* [Better plugin management](https://forum.obsidian.md/t/better-plugin-management-with-folders-and-links/17568/2) to allow for grouping plugins by topic, especially linking plugins to particular workspaces, is a neat suggestion.  

## Appearance

* The [Shimmering Focus](https://github.com/chrisgrieser/shimmering-focus) theme is now a minigame. "Hardcore mode" doesn't have a settings button, hotkey descriptions, or most UI elements. "Madness mode" is basically a short puzzle game, purely made out of CSS hacks. There are more [details on Discord](https://discord.com/channels/686053708261228577/855181471643861002/972799254882058290). 
- [Modern Dark](https://github.com/roberts-code/obsidian-theme-modern-dark) by `@roberts-code`  is new :) 
* [Willemstad v0.5.0 Jordaan](https://github.com/tingmelvin/willemstad-x/releases/tag/v0.5.0) got its biggest update yet; it now has callout styling, new icons, prettier highlights, and more. 
* [Minimal 5.2](https://github.com/kepano/obsidian-minimal/releases/tag/5.2.0) added block widths to Live Preview, new sidebar tab styles, active line highlighting, custom font headings, and more. Minimal 5.2.4 allowed for all the helper classes for tables to be activated globally via the Style Settings plugin. 
* [Primary v.1.4.7](https://github.com/ceciliamay/obsidianmd-theme-primary/releases/tag/v.1.4.7) added progress bar styling, slides support, and more. 
* [Prism v2.1.0](https://github.com/damiankorcz/Prism-Theme/releases/tag/2.1.0) now officially supports mobile, has styling for query blocks, new custom icons, new style settings, and more. It does come with a few breaking changes for graph colors and header margins. 

## Ancillary Code

* Here's a powershell script to [add extra time to a task and update the time of all future tasks](https://www.reddit.com/r/ObsidianMD/comments/ul4gvm/i_made_a_powershell_script_for_use_with_the_day/) for the Day Planner plugin. 

## Guides

* Bob Doto has a new [Building a Zettelkasten for Creative Expression](https://bobdoto.computer/zettelkasten-101 ) course starting in June; registration is limited to 20 people. 
* Here are some neat [periodic note templates](https://github.com/mulfok/periodic-note-templates), including a habit tracker, weather tracker, and work log. 
* Here's a step by step guide for [how to create a personal movie database](https://minimal.guide/Guides/Create+a+movie+database) using QuickAdd and Minimal.
* Here's a guide for [how to do a weekly reflection](https://www.youtube.com/watch?v=NVu7EWLE34s). 
* Here's a guide for [how to make Obsidian useful for filling out forms](https://jamierubin.net/2022/05/10/practically-paperless-with-obsidian-episode-29-filling-out-forms/). 

## Discussions

* Here's a good discussion from Reddit about how to [sandbox Obsidian to limit potentially malicious plugins](https://www.reddit.com/r/ObsidianMD/comments/unbwdm/sandboxing_obsidian_to_protect_from_malicious/) (although honestly I think the biggest risk from plugins is likely to be accidental deletions, not people sending data back to the developer). 
* Here's a discussion about [whether people still tweak their workflows after a year or so](https://www.reddit.com/r/ObsidianMD/comments/umgcu5/people_whove_been_using_obsidian_for_over_a_year/) of using Obsidian. 
* Here's a discussion about [what people store in Obsidian](https://www.reddit.com/r/ObsidianMD/comments/um2xlv/what_exactly_do_you_store_in_obsidian/). 

## Ancillary Tools

* the [Raycast Obsidian extension](https://www.raycast.com/marcjulian/obsidian) got a bunch of updates, like improved support for Templater and new preferences and lists of pinned notes. 

## Housekeeping

Thanks for the well wishes, everyone! I've still got a lingering cough from my bout with COVID, but my kid is allowed to go back to school on Monday and I'm finally able to sleep through the night without medicine, and more importantly, I can think straight again. 