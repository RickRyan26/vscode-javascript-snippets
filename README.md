<h1 align="center">
  <br>
    <img align="center" src="img/logo.png" width="200">
  <br>
	<br>
  JavaScript Snippets for Humans
  <br>
  <br>
</h1>
<h4 align="center">Descriptive, easy to find JavaScript snippets, without nonsense abbreviations.</h4>

<p align="center">
<img src="https://img.shields.io/static/v1?logo=visual-studio-code&label=made%20for&message=VS%20Code&color=0000ff" alt="Made for VSCode">
<img src="https://img.shields.io/visual-studio-marketplace/v/robole.javascript-snippets?logo=visual-studio-code&color=ffa500" alt="Visual Studio Marketplace Version">
<img src="https://img.shields.io/static/v1?logo=visual-studio-code&label=size&message=11KB&color=008000"
alt="Extension file size in bytes">
<img src="https://img.shields.io/visual-studio-marketplace/r/robole.javascript-snippets?logo=visual-studio-code&color=yellow" alt="Visual Studio Marketplace Rating">
<img src="https://img.shields.io/visual-studio-marketplace/d/robole.javascript-snippets?logo=visual-studio-code&color=blue" alt="downloads"/>
<img src="https://img.shields.io/visual-studio-marketplace/i/robole.javascript-snippets?logo=visual-studio-code&color=blue" alt="installs"/>
<img src="https://img.shields.io/static/v1?label=built%20with&message=good%20vibrations&color=purple" alt="Built with"/>
<a href="https://ko-fi.com/roboleary"><img src="https://img.shields.io/badge/Buy%20me%20a%20coffee-$4-orange?logo=buy-me-a-coffee" alt="Buy me a coffee"></a>
</p>

Most snippet collections resemble bash aliases. You have a list of abbreviations such as "imp", "clg", "fre", and so on. You must learn these to use them. 🤕

There is a better way!

Snippets are not confined to using a single word as the trigger (prefix). We can be more descriptive, and make them easier to discover.
For example, you want to find an array function, but not sure which to use, just type "arr" and you get a list with descriptions:

![example with suggested array functions](img/array-functions.gif)

## Activation

These snippets are available for the follow [language identifiers](https://code.visualstudio.com/docs/languages/identifiers):
- `javascript`
- `javascriptreact`
- `typescript`
- `vue`
- `svelte`

## Snippets

You can install the [Snippets Ranger extension](https://marketplace.visualstudio.com/items?itemName=robole.snippets-ranger) to view the full list of snippets inside VS Code.

I didn't repeat any of the builtin JavaScript snippets.

Here is an excerpt:

## Installation

1. The extension is listed in the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=robole.javascript-snippets) and [Open VSX Marketplace](https://open-vsx.org/extension/robole/markdown-snippets) where you can download or install it directly.
1. From the Command-line: Run the command `code --install-extension robole.javascript-snippets`.

## FAQ

### 1) Where do the standard markdown snippets come from?

There is a set of snippets for the standard markdown syntax installed with VS Code as part of the built-in markdown extension. [This is the source file](https://raw.githubusercontent.com/microsoft/vscode/94c9ea46838a9a619aeafb7e8afd1170c967bb55/extensions/javascript/snippets/javascript.code-snippets).

The [Snippets Ranger extension](https://marketplace.visualstudio.com/items?itemName=robole.snippets-ranger) will show the built-in snippets in a good-looking webview.

### 2) How do I use the snippets?

To insert a snippet, you can just type one of the prefixes in a markdown file, and you will be offered a completion suggestion. The setting `Editor: Snippet Suggestions` controls whether snippets are shown with other suggestions and how they are sorted. By default, they are shown inline.

Alternatively, you can open the Command Palette (`Ctrl+Shift+P`) and run the command "Insert Snippet", which presents you with a list to choose from.

### 3) How do I add shortcuts for the snippets?

Run the command `Preferences: Open Settings (UI)` to open the keyboard shortcuts config. Add an new object to the array such as this:

```JSON
[

	{
		"key": "ctrl+t",
		"mac": "cmd+t",
		"command": "editor.action.insertSnippet",
		"when": "!editorReadonly && editorLangId == javascript",
		"args": {
			"langId": "javascript",
			"name": "arrow function"
		}
	}

]
```

The `args.name` property <u>must exactly match</u> the snippet name.

### 4) Where can I learn more about snippets?

You can read my comprehensive guide on Snippets on FreeCodeCamp: [Visual Studio Code Snippets – the Definitive VS Code Snippet Guide for Beginners](https://www.freecodecamp.org/news/definitive-guide-to-snippets-visual-studio-code/). It's not just for beginners! 😉

## Show gratitude

If you are happy with the extension, please star the repo, and leave a review to help others find it. 🌟🌟🌟🌟🌟

You can [buy me a coffee](https://ko-fi.com/roboleary) if you would like to enable me to make more great open-source software and tutorials. ☕🙏

[![buy me a coffee on kofi](img/buymeacoffee.png)](https://ko-fi.com/roboleary)