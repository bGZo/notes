---
created: 2024-12-09T12:00:00
modified: 2024-12-24T09:54:17
---

Okey, I know it's ridiculous and hard to say: **I give up [[logseq]]**, ending up the 3 years usage career. Honestly, I'm not good enough using this tool, such as IDK when they add the support of markdown YAML properties, even though I always read changelog of it. [^earier-logseq]

## Problems

### Markdown version (following using MV as abbr)

#### Hard to build huge system

Based on several features applied, the whole construction of PKM also changed several times, which means **downward compatibility** is huge and difficult. It's something kind of wasting time.

I break my PKM three times, and finally I give up it. Since enabled telegram inbox + telegram RSS bot, I was fell into the hell of poor performance.

#### Hard to share & read with raw format

The active user on community I know is xxx, which shared opinions via LOGSEQ format.

How to comment? I agree this is a simple and awesome way. But it's really hard to read and understand as well.

### Database version

Now official has announced,[^announced] and alpha test has started. The double preview way is available following:

- https://logseq-db-demo.pages.dev/
- https://test.logseq.com/#/

I meet some imported problem, such as `excludelist` config on `config.edn` would not ignore when imported, `no uuid found for page name nil`.

When I delete the pdf annotations, and imported most of them, I was so excited to try reviewing notes on database version. I sadly notice:

- **Query is slower** then MV.
- **Page is easier to be stuck** then MV.
	- Breaking up browser and need to be relaunched.
- **Editing block is so difficult** as same as MV.

Compared to MV, database is not solving any problems on performance. And you are losing the support of  `template`, `schedule`, sync local pure markdown file (cooperated with other tools base on pure text), and desktop plugins support.

They really have a very very long way to reach. I have no time to wait them.

## Switch [[obsidian]] Notes

### Replace all properties `::` with `yaml` format

replace `yaml` to `::` is easy. But using regex to replace `::` to `yaml` is a hard thing.

But there is something worth to try

```diff
-Org-mode syntax
#\+BEGIN_PIN\n([ ]+)
#\+BEGIN_PINNED\n([ ]*)
#\+BEGIN_PIN\n([ ]+)
#\+BEGIN_EXAMPLE\n([ ]+)
#\+BEGIN_NOTE\n([ ]+)
#\+BEGIN_WARNING\n([ ]+)
#\+BEGIN_IMPORTANT\n([ ]+)
+>[!tip]\n$1

- no used property
[ ]*closed: .*\n

- shadule time
^\s*\* State "DONE" from "WAIT".*$\
[ ]+:LOGBOOK:[\n]+[ ]+:END:\n([ ]+)
[ ]+:LOGBOOK:\n[ ]*:END:\n([ ]+)

- no use break line
^-\n
\n---\n[^\n ]
```

### Properties
#### Date not link journals
#### Date format shown

[Properties: let the user customize the way Dates/Times are displayed (independently from OS) - Feature requests - Obsidian Forum](https://forum.obsidian.md/t/properties-let-the-user-customize-the-way-dates-times-are-displayed-independently-from-os/64139/34?page=3)

#### Value cannot be a image

That not impossible with `![]()` as value. Yet use link and format it on dataview query.

https://forum.obsidian.md/t/how-do-you-dynamically-embed-a-picture-tied-to-a-metadata-value/54011

### Plugins
#### Web Cliper

Save as `import.json` to import.

```json
{
	"schemaVersion": "0.1.0",
	"name": "Default",
	"behavior": "create",
	"noteContentFormat": "{{content}}",
	"properties": [
		{
			"name": "created",
			"value": "{{date|date:YYYY-MM-DDTHH:mm:ss}}",
			"type": "date"
		},
		{
			"name": "created-link",
			"value": "[[{{date|date:YYYYMMDD}}]]",
			"type": "text"
		},
		{
			"name": "source",
			"value": "{{url}}",
			"type": "text"
		},
		{
			"name": "type",
			"value": "archive-web",
			"type": "text"
		}
	],
	"triggers": [],
	"noteNameFormat": "~{{title}}",
	"path": "archives/clippings"
}
```

#### Reminder

#### Chinese Tools

#### Turn to page

#### Agenda

#### Markmap

#### Web parser

### Hotkey

- `alt+a/d` outliner move
- `ctrl+enter` task switch
- `command+1` heading switch
- [Easily switch between source mode <-> live preview <->](https://forum.obsidian.md/t/easily-switch-between-source-mode-live-preview-preview/27151)
- [Is there a plugin for changing blocks locations? : r/ObsidianMD](https://www.reddit.com/r/ObsidianMD/comments/ydc48j/is_there_a_plugin_for_changing_blocks_locations/)

### Graph
- local graph
- global graph
- [Global graph view: open with currently active note highlighted - Feature archive - Obsidian Forum](https://forum.obsidian.md/t/global-graph-view-open-with-currently-active-note-highlighted/245/13)

### Miss macros
- [Iframe - Help - Obsidian Forum](https://forum.obsidian.md/t/iframe/14296/3)
- [Simple macros? - Help - Obsidian Forum](https://forum.obsidian.md/t/simple-macros/44009)
- [What are the creative ways to use iframes .... : r/ObsidianMD](https://www.reddit.com/r/ObsidianMD/comments/1aufiav/what_are_the_creative_ways_to_use_iframes/)

### PDF annotations
- [Handle PDFs Natively in Obsidian – Curtis McHale](https://curtismchale.ca/2023/11/08/handle-pdfs-natively-in-obsidian/)

### CSS
#### Image size

```css
/* via: https://forum.obsidian.md/t/resize-image/6517/17
*/
.markdown-preview-view img[alt="sm"] {
  width: max(300px,30%);
  max-height:auto;
}
.markdown-preview-view img[alt="md"] {
  width: max(500px,50%);
  max-height:auto;
}
.markdown-preview-view img[alt="lg"] {
  width: max(1080px,70%);
  max-height:auto;
}
```

#### Iframe

> [!warning]
> Some video cannot be iframed.
> That would be unavailable.
> If iframe the whole page, the video will be played automatically.
> via: https://forum.obsidian.md/t/youtube-video-unavailable/61107
> https://stackoverflow.com/questions/44839312/disable-auto-play-in-youtube-embeded-code


#### Code block with no wrap

- https://forum.obsidian.md/t/disable-word-wrap-for-code-blocks/13210/16
### Query

#### Exclude some folder

```diff
-path: foldername
```

- https://www.reddit.com/r/ObsidianMD/comments/w6p5xc/how_do_i_exclude_templates_from_this_dataview/
- https://forum.obsidian.md/t/exclude-templates-folder-from-file-explorer-graph/5012/7

More Query

- https://publish.obsidian.md/tasks/Queries/About+Queries
- https://forum.obsidian.md/t/dataview-how-to-specify-the-order-of-properties/69721

### Others
- Use spaces instead of tab: https://forum.obsidian.md/t/use-tabs-off-only-replaces-tabs-with-spaces-in-lists/3583
- [Show location of currently open file - Feature requests - Obsidian Forum](https://forum.obsidian.md/t/show-location-of-currently-open-file/41903)
- [Any way to disable line wrapping in code blocks? : r/ObsidianMD](https://www.reddit.com/r/ObsidianMD/comments/zh0ih2/any_way_to_disable_line_wrapping_in_code_blocks/)

[^earier-logseq]: in earlier version, they released fast,  I used to learn feature via changelog. the hierachy is using via twitter, the macros via community discuss. and even someone analyze the logic of language, break it into pieces, and try explain it with Logseq.
[^announced]:[Why the database version and how it's going? - Announcements - Logseq](https://discuss.logseq.com/t/why-the-database-version-and-how-its-going/26744/25)