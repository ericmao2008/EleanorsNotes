---

---

- [i] Intended for publication with [[Obsidian Roundup]]

## In The Community

* Maggie Appleton's [list of digital gardens](https://github.com/MaggieAppleton/digital-gardeners) (& tips & tools) was shared, there are a bunch of nice examples there. 
* `@shabegom` will be giving a community talk about their plugin, [Buttons](https://github.com/shabegom/buttons), today at 18:00 (CET).

## Obsidian Updates

* [v0.12.14 for Insiders](https://forum.obsidian.md/t/obsidian-release-v0-12-14-insider-build/23046) comes with bugfixes and a nifty new utility to rename headings with the context menu, which will _update links_. This is very powerful, especially when coupled with the [block ref counter plugin](https://github.com/shabegom/obsidian-reference-count/releases/tag/0.1.0) that is currently in beta. 

## Plugin News

Licat went through and approved a bunch of plugins, so if you were waiting for something to be in the community list, double-check and see if it's there now. 

### Updates

* Admonitions 6.3.0 allows users to upload images to use as the admonition icon.
* The Toggl Track plugin needs to be updated to v0.2.5 to reduce load on the Toggl Track API. 
* [Excalidraw v1.2.15](https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.2.15) supports CTRL+hover-preview of links in drawings. [v1.2.16](https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.2.16) fixes a rare race condition and improves fullscreen mode. 
* The Readwise _Community_ Plugin is now at [v0.0.9](https://github.com/renehernandez/obsidian-readwise/releases/tag/0.0.9) with some QOL improvements and bugfixes. 

### New

* [Obsidian Annotator](https://github.com/elias-sundqvist/obsidian-annotator) is a plugin for reading and annotating PDFs and EPUBs in Obsidian. It's based on hypothes.is but stores annotations in a local markdown file. 
* [Obsidian Card View Mode](https://github.com/yo-goto/obsidian-card-view-mode) has some nifty sliding panes style views and the ability to grey out unfocused panes. 
* [Open With](https://github.com/phibr0/obsidian-open-with) lets you open notes with other software (like Typora or Notepad) using the command palette. 
* [Obsidian Image Toolkit](https://github.com/sissilab/obsidian-image-toolkit) lets you click on an image and rotate it in preview. 
* [Hover External Link](https://github.com/jamiebrynes7/obsidian-hover-external-link) lets you get a tooltip with the website URL when you hover over an external link in preview mode. It's another one of those nice little quality of life things. 

**Task Management:**

* The [Task Archiver](https://github.com/ivan-lednev/obsidian-task-archiver) will automatically move completed tasks to an "Archived" heading. It's meant to be a (partial for now) implementation of the similar org-mode feature.
* There's a new [Trello integration](https://github.com/OfficerHalf/obsidian-trello/) that can retrieve data from Trello and display and add comments. Note that this requires the MetaEdit plugin. 
* The [Reminder](https://github.com/uphy/obsidian-reminder) plugin will notify you of tasks at a time you specify. 
**Prettification:**
* [Obsidian banners](https://github.com/noatpad/obsidian-banners) adds pretty banners to your notes. 
* [Obsidian Icon Folder](https://github.com/FlorianWoelki/obsidian-icon-folder) lets you add icons to folders without having to mess with emojis or CSS. 
* [Code Mirror Options](https://github.com/nothingislost/obsidian-codemirror-options/releases/tag/0.0.2) allows for some fancy appearance alterations and selector improvements, like changing the color of selected text, and better syntax highlight consistency. 
* [Code Block Enhancer](https://github.com/nyable/obsidian-code-block-enhancer) adds a copy button, linenumber, and language name for code blocks when in preview mode. 

**Commands:**

* [Command Alias](https://github.com/yajamon/obsidian-command-alias-plugin) lets you add aliases to commands. 
* [Editor Commands Remap](https://github.com/c4ctus5/editor-commands-remap) lets you map hotkeys to editor commands like `goLeft` and `swapLineUp`. 

**Calendar stuff: **

* [Jump to Date](https://github.com/TfTHacker/obsidian42-jump-to-date) is a popup calendar for quickly navigating daily notes. 
* [Weekly note](https://github.com/maloneya/ObsidianWeekly) semi-automates weekly note templates. 
* [Daily folder](https://github.com/NemoAndrea/obsidian-daily-folder) adds some improvements to the core daily note functionality, like better next/previous functionality. 

**Advanced: **

* [Shell Commands](https://github.com/Taitava/obsidian-shellcommands) lets you run terminal/shell commands from within Obsidian. Desktop only. 
* [CustomJS](https://github.com/samlewis0602/obsidian-custom-js)

_Remember: You can manually install plugins that aren't in the community list by copying the main.js, manifest.jso and (optionally) the styles.css files into {vault}/.obsidian/plugins/{plugin-folder}. It can then be enabled like any other plugin (you may need to refresh the list first). Usually these files can be found at the GitHub repo under Releases. Note, though, that this is not as safe as waiting for them to go through code review._

### For Developers

* `@shabegom` created a [hot reload for mobile](https://github.com/shabegom/obsidian-hot-reload-mobile/releases/tag/1.0.2) thing. You should update `pjeby`'s Hot Reload for desktop before using it, I think. There was a discussion about it [here](http://discordapp.com/channels/686053708261228577/840286264964022302/879405215235854386) but if we're being honest it's way over my head. 

## Workflow Stuff

* `@d.w.frank` shared a [series of blog posts](https://dwf.bigpencil.net/series/obsidian/) about how they use Obsidian, along with how they're using it for a job search.
* `@pseudometa` shared all the [documentation](https://github.com/chrisgrieser/shimmering-obsidian) for their Alfred workflow for Obsidian (mac-only). It covers plugin search, OCRing screenshots and toggling CSS snippets. 
* `Moonbase59` [updated the clipit script](https://forum.obsidian.md/t/clipboard-snippets-in-your-inbox-for-later-review-even-when-obsidian-closed/22850) for getting clipboard snippets into Obsidian to include YAML frontmatter with date and tags. It also has better Pandoc options, daily clipboards, and bugfixes. 

## Feature Requests

* There was some discussion about [increasing contrast of icons](https://forum.obsidian.md/t/enhance-default-color-contrast-of-the-icons/23045/3) and how a theme that prioritizes accessibility would be valuable for the community.
* It would be neat if there was a plugin to add functionality for [choosing a folder whenever a new note is created from a link](https://forum.obsidian.md/t/choose-a-folder-whenever-a-new-note-is-created-from-a-link/23177). 

## Appearance

* `@SkepticMystic` shared a way to make [images zoom on hover](https://discord.com/channels/686053708261228577/722584061087842365/878721627427323974) which is handy for slideshows. 
* `@Moonbase59` shared some css to [improve the GarbleText functionality](https://forum.obsidian.md/t/garble-text-on-screen-to-hide-private-info-with-added-features/23143). He also updated the [clean embeds css](https://forum.obsidian.md/t/meta-post-common-css-hacks/1978/394) (here's for [all](https://forum.obsidian.md/t/meta-post-common-css-hacks/1978/411)). 
* `@curtismcshale` shared a video about how they [use daily notes](https://youtu.be/14GSuqWh4oU). 
* This set of [icons for iOS/Mac](https://www.reddit.com/r/ObsidianMD/comments/l6amlf/three_icons_for_a_better_mac_experience/) got resurfaced again. Here's [another new icon](https://twitter.com/Gavmn/status/1431286249814315010?s=20). 

## Knowledge Management

* I wrote a [quick-reference guide for evaluating the reliability of stuff you read on the internet](https://eleanorkonik.com/evaluating-references/). 
* [How to Take Smart Notes in Obsidian](https://knowledgework.substack.com/p/how-to-take-smart-notes-in-obsidian) by `@joshduffney` got resurfaced a couple of times as a nice primer. 
* `@SlRvb` shared an incredibly comprehensive [explanation](https://forum.obsidian.md/t/slrvbs-mediadb-setup/23227) of how they use Obsidian as a media database. 
* There was a nice discussion on Reddit about the value of [using camelCase for tags](https://www.reddit.com/r/ObsidianMD/comments/pbzqia/tags_or_tags/). I'm actually really terrible about doing this even though I know it's better. Actually there were a bunch of discussions about tags on reddit, including the perennial [links versus tags](https://www.reddit.com/r/ObsidianMD/comments/pb0rrv/tags_what_is_the_difference_between_tagging_with/) discussion. Here's another one on [the Obsidian forum](https://forum.obsidian.md/t/how-do-you-use-tags/23172/5), which I contributed to. Also here's another one from Reddit about whether to place [tags at the top or the bottom](https://www.reddit.com/r/ObsidianMD/comments/pacv14/tags_on_top_of_note_or_bottom/) of a file. 
* `@blizzingout` shared their for-medical-use variant of zettelkasten, called "[CSI](https://discord.com/channels/686053708261228577/710585052769157141/879686732675706911)," which is a nice modern practical update on the methodology that I quite like. It uses sources, inputs, summaries and "connectors" to link things together and it's a nifty new paradigm. 
* `@otolith` shared their "[digital country estate](https://discord.com/channels/686053708261228577/710585052769157141/879520742063112273)," an expansion of the "digital garden" that works a bit better for clinical neuroscience than a publication-focused "digital garden." `@PaperbackCook` also shared another [alternative](https://discord.com/channels/686053708261228577/710585052769157141/879140427607973898) to the "digital garden" metaphor, involving toilet paper emojis. 
* Here's how Tara made a [dictionary using Obsidian](https://tamethestars.wordpress.com/2021/08/24/how-to-make-a-dictionary-with-obsidianmd/)

## Ancillary Tools

* [Mathpix](https://mathpix.com/) will turn handwritten formulas into LaTeX formatting. [LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR/) has better local-first privacy but apparently isn't quite as good, so, tradeoffs. 

## Housekeeping

Awhile back, somebody requested a community talk about project management for fiction, with bonus points if the talk could cover managing marketing in Obsidian. I didn't pick it up at first because I didn't feel qualified, but now I've got [The Iceberg](http://newsletter.eleanorkonik.com/), my weekly newsletter where I share short fiction & the nerdy history & obscure biology research that supports the stories. It's doing pretty well, so I decided to go ahead and give the talk... which meant documenting things. That's how last week's article about the gardening metaphor for notetaking got started. 

Well, this week I set out to update my "How I use Obsidian for Writing" article to sort of consolidate all of different quirks of my personal knowledge management system. You can see the [saga of how the article metastasized on Twitter](https://twitter.com/EleanorKonik/status/1429850365747466248) but since apparently I'm writing a book (16,000 words and counting!) and I don't know a ton about nonfiction publishing, if you _do_ I would love recommendations / referrals for things like decent nonfiction copy editors, resources for typesetting, viable alternatives to Amazon, etc. Thanks! 