# atom markdown editor

Makes the markdown editor look more like the final result.

## Installation

Copy [`style.less`](https://raw.githubusercontent.com/pfgithub/atom-markdown-editor/master/style.less) to your atom user stylesheet. (Edit > Stylesheet...)

- Requires the [`language-markdown`](https://github.com/burodepeper/language-markdown) package for markdown parsing.
- Any dark syntax theme should work, default settings were built with the [`city-lights-syntax`](https://github.com/Yummygum/city-lights-syntax-atom) theme.
- [`move-cursor-improved`](https://github.com/susisu/move-cursor-improved) is recommended for making the cursor up/down work properly with non-monospace fonts.

Recommended Settings:
```cson
"*":
	editor:
		showIndentGuide: true # OPTIONAL. The indent guide is customizeable in the style config.
		showInvisibles: true # OPTIONAL. These can be hidden in the style config
		softTabs: false # OPTIONAL. Hard tabs work better with many markdown elements, like lists.
		tabLength: 4 # OPTIONAL. The indent guide is set up for 4 width hard tabs by default
	whitespace:
		removeTrailingWhitespace: false # OPTIONAL. So two spaces at the end of lines are not removed
```

Configure the stylesheet with the variables and mixins at the top.

[![Demo](https://i.imgur.com/VrI99Mk.png)](https://pfgithub.github.io/atom-markdown-editor/DEMO)  
(click to view demo rendered by github)

## Known Issues

Some markdown features are not supported by the markdown parser used.

***bold italic***, ~~**bold strikethrough**~~

		doubletab code blocks

horizontal line titles
---

```markdown
Some markdown features are not supported by the markdown parser used.

***bold italic***, ~~**bold strikethrough**~~

		doubletab code blocks

horizontal line titles
---
```

