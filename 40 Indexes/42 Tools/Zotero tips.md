- [Jenks' quickstart youtube guide for Zotero](https://www.youtube.com/watch?v=_Fjhad-Z61o) 
- [Argentum's explanation of why reference managers & citekeys are useful](https://discord.com/channels/686053708261228577/722584061087842365/814168053541240892)
- [longform guide on how to do Zotero well](https://ikashnitsky.github.io/2019/zotero/) -- mirrored [here](https://habr.com/en/post/443798/)
- [attaching pdfs instead of downloading them](https://www.zotero.org/support/attaching_files)
- [tips shared via Discord](https://discord.com/channels/686053708261228577/722584061087842365/837390206503092234)
	* [MDNotes placeholders to make use of inline fields in dataview](https://discord.com/channels/686053708261228577/722584061087842365/836340716485476373)
- [Zotero -> zotfile -> mdnotes -> obsidian -> dataview Workflow](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536)
- [When to use mdnotes wildcards instead of placeholders?](https://publish.obsidian.md/argenos/tools+%26+software/zotero/zotero-tips/When+to+use+mdnotes+wildcards+instead+of+placeholders%3F)
- there are both placeholders (e.g. `{{citekey}}`) and wildcards (e.g. `%(citekey)` for all fields. The first are a quick way to get `- <name of field>: <field content>` and allows you to apply some formatting. The 2nd one are the raw contents of that field. Zotero is a bit weird with fields and not all types of items have all fields, so, the important thing to remember is that `{{placeholders}}` are removed from your template if the item you're exporting doesn't have it, while `%(wildcards)` will be left there, and should be used sparingly for things you know all items will have, e.g. title, authors, citekey, date (although in the talk we saw podcasts don't have date for some reason)
