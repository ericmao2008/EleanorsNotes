---

---

- [i] Intended for publication with [[Obsidian Roundup]]

## Obsidian Updates
* The [Insider Build](https://forum.obsidian.md/t/obsidian-release-v0-12-10-insider-build/20523) is up to 12.10 now. It’s mostly sync fixes, but that means that since hotkeys are now stored in a separate file, if you’re using Obsidian on multiple devices you might notice that your hotkeys will disappear on non-upgraded Obsidian instances when using Obsidian Sync to sync your app config. To migrate, upgrade Obsidian and turn on the hotkeys sync flag to receive the hotkeys, then restart Obsidian.

## Plugin News

### New
* My hero `@mrjackphil` is back creating [plugins by request](https://forum.obsidian.md/t/uuid-for-note-links-in-url-scheme/14617), this time tackling a plugin that will [create and open UID notes by UID](https://github.com/mrjackphil/obsidian-note-uid). Currently, it only opens notes by UID. Hopefully soon it’ll the ability to generate those UID for notes.
* [Enhanced Mindmaps](https://github.com/MarkMindCkm/obsidian-enhancing-mindmap) can do a lot of nifty stuff for, well, making better mindmaps. 
* [tq v0.1.0](https://github.com/tgrosinger/tq-obsidian) is a task management plugin that uses a separate note to back each task and renders them in customizable code blocks. 

### Updates
* [Breadcrumbs now has support for Juggl-formatted links](https://github.com/SkepticMystic/breadcrumbs). It also supports multiple indexes. 
* [Tracker v1.8.0](https://github.com/pyrochlore/obsidian-tracker) has support for month view, displays color based on a particular value, and all around is starting to look really incredible for, well, tracking things based on metadata. 
* [Better Word Count 0.7.0](https://github.com/lukeleppan/better-word-count) has some speed improvements, customizable status bar counters, and stats for the day. I don’t think I’ve ever updated a plugin so fast!  
* [File Tree Alternative](https://github.com/ozntel/file-tree-alternative/releases) now lets you search from within its file list view. 

### Magic
* I’m going to mangle this explanation, but `@kaelri` [shared](https://discordapp.com/channels/686053708261228577/694233507500916796/854541472761905162) how they make [project cards](https://gist.github.com/kaelri/f7427fef75a375a453faa7e9c030e254) using Templater and Dataview and it got bookmarked 66 times, so check it out if you’re somebody who enjoys content cards. One way to think of it is that it’s like a prettier / less table-like dataview view (thanks for walking me through it, `@anthonybaker`). 
### Under The Radar
* There was a fun discussion of everybody’s [top 3 favorite plugins](http://discordapp.com/channels/686053708261228577/707816848615407697/861911446212444160) that I recommend checking out if you’re not sure where to start. Plus, it’s fun to see how different people have such varied use-cases. 
### For Developers
* If you are trying to debug plugins for android, you need to have [Android Debug Bridge](https://developer.android.com/studio/command-line/adb) on your computer installed; on your android phone you have to enable ADB (it's under developer settings – tap the build number three times to get these settings); then connect the phone to your computer over USB; open chrome (or chromium based browser should also work) and type `chrome://inspect` in the browser. Open obsidian on your phone, then it should appear. 

## Workflow Stuff
* Folks with Obsidian mobile on their android device might benefit from these tips about [how to keep an app permanently running in the background](https://www.androidcentral.com/how-keep-app-permanently-running-background-galaxy-s20). It makes the new sharing features a bit nicer. 
* `@cotemaxime` shared the second part of their [productivity system explainer](https://www.maximecote.me/blog/my-productivity-system-executing/). It’s mostly task management and things on the weekly scale.
* `@tallguyjenks` shared their [kindle to Obsidian](https://youtu.be/GKj6y7nKlxY) workflow on YouTube. 
* `@hamster` shared a quick and dirty way to get an obsidian markdown file into .docx format if you don’t want to mess with pandoc or have to deal with footnotes: click on the 3 dots of the note - export to pdf, hen drag the pdf into google docs and then open it as a google doc and then save it as a docx. 
* There was a discussion of [daily note templates](http://discordapp.com/channels/686053708261228577/694233507500916796/861616486261850114) in Discord. 
* `@sashinexists` shared a [script](http://discordapp.com/channels/686053708261228577/722584061087842365/860727328597999636) that takes in a better bibtex json file and from it generates markdown notes and organises them into folders based on type in your vault.
* `@joshduffney` merged Cal Newport's time-blocking system into Obsidian and created [a short video on it](https://www.youtube.com/watch?v=4j4hG_0AoWs). 
* `@Thomas Curro` shared how to [automate filing notes into folders with templater](https://www.youtube.com/watch?v=VPAGohAwiow). 
* Reddit had an interesting discussion about how people [use Obsidian to replace various other tools](https://www.reddit.com/r/ObsidianMD/comments/ofp9s2/how_many_tools_has_obsidian_replaced_for_you/), with an additional thread about [what plugins are useful when migrating from Notion](https://www.reddit.com/r/ObsidianMD/comments/ofqxes/people_who_have_switched_from_notion_to_obsidian/). 
* Keep Productive hosted Santi Younger for a sort of updated [2021 Obsidian Intro](https://www.youtube.com/watch?v=oaDkQl2zclY). 
## Feature Requests
* A feature request to make it possible for [opening certain files to default to a particular mode](https://forum.obsidian.md/t/opening-certain-files-defaults-to-certain-modes/20600) was made. 
* This feature request to create a “heatmap” to [color-code the graph view based on how recently a file & its linked associations was edited](https://forum.obsidian.md/t/graph-colourisation-according-to-brain-entropy/20402) is a really neat idea. 
## Appearance
* The [Yin and Yang theme](https://github.com/chetachiezikeuzor/Yin-and-Yang-Theme) got an update. Among other things, `@chetachi` added base hue and saturation customization! You can now easily and uniformly change the base colors to the theme. Yin and Yang is an excellent theme all around but is also one of the few I’m aware of that is optimized for mobile. 
* This reddit thread is a really nice collection of different ways to [color code text](https://www.reddit.com/r/ObsidianMD/comments/oeq7ae/i_have_a_question_about_text_colors/). 
## Knowledge Management
* There was a nice [reddit thread](https://www.reddit.com/r/ObsidianMD/comments/ocgmsh/recipes/) discussing how to use Obsidian for managing recipes. 
* Here’s an [interesting read about history of notetaking](https://boffosocko.com/2021/07/03/differentiating-online-variations-of-the-commonplace-book-digital-gardens-wikis-zettlekasten-waste-books-florilegia-and-second-brains/) shared by `@danieltomasz`) 
* This [YouTube video](https://www.youtube.com/watch?v=7ik0JNnoXBc) about personal knowledge graphs in various personal knowledge management software was shared. It was part of a conference and is pretty thought-provoking. 
* Here’s a reddit discussion about resources for [how to take book notes in Obsidian and share them on a blog](https://www.reddit.com/r/ObsidianMD/comments/ogmgnn/book_notes_in_obsidian/).  

## Ancillary Tools
* If anyone is looking for a Working Copy alternative (aka iOS only), [Polygit](https://www.polygitapp.com/) is $2/mo or $10/year and lets you clone a repo directly into the Obsidian folder. (via `@Krafty`) 
* Anecdotally, MGit is the favored git-for-mobile option for Android, but I don’t think anybody has figured out a way to auto-sync a git repo on android (although the latest mobile update might have changed that, so if you get autosync of a git repo working on mobile please reach out).  
