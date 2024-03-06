---
dg-publish:
---
# Welcome to the Astral Café.
This repository is the basis for [community documentation](https://docs.astral.cafe/) for Google Sheets. If you wish to contribute, feel free to make a pull request or [contact me over Discord](https://discord.com/users/365169403316142090).

The site is published using the [Obsidian Digital Garden](https://github.com/oleeskild/Obsidian-Digital-Garden) plugin for [Obsidian](https://obsidian.md/). You can find the documentation for the Digital Garden plugin [here](https://dg-docs.ole.dev/).
# Note Guidelines
In order to work with the Digital Garden plugin, there are a few conventions each note should follow. All notes should be markdown files (`.md`).
## Header
This goes at the beginning of each file.
```
---
title: Example
tags:
  - example-tag
dg-publish: true
dg-permalink: example
---
```
- `title` - The title of the note. When published, the title goes at the top of the page.
- `tags` - Relevant tags for the note. Notes can have multiple tags, but they should be formatted on new lines with a leading hyphen as seen above.
- `dg-publish` - This should be `true` if you want the note to be published or `false` if not.
- `dg-permalink` - This sets the note's URL on the site. It should be relatively short.
## Callouts
The Digital Garden plugin supports [callouts](https://help.obsidian.md/Editing+and+formatting/Callouts). There are no specific conventions for when they should be used, as long as it makes sense.
## Code Blocks
Code blocks should use the `xls` syntax highlighter.
## Wikilinks
The Digital Garden plugin supports [wikilinks](https://help.obsidian.md/Linking+notes+and+files/Internal+links). Use them when possible, and don't be afraid to make dead links to be filled later.