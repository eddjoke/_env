# VSCode

## User Settings

```json
{
  "search.exclude": {
    "**/node_modules": true,
    "**/public": true
  },
  "editor.tabSize": 2,
  "editor.rulers": [120],
  "editor.wordWrapColumn": 120,
  "editor.wordWrap": "wordWrapColumn",
  "editor.formatOnSave": true,
  "eslint.autoFixOnSave": true,
  "prettier.eslintIntegration": true,
  "workbench.colorTheme": "One Dark Pro",
  "files.autoSave": "onFocusChange",
  "emmet.triggerExpansionOnTab": true,
  "emmet.showExpandedAbbreviation": "always",
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "vue-html": "html"
  }
}
```

## Plugins

Must have:

* [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager) - project manager
  * `Shift + Alt + P` - to list projects
* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - ESlint support
* [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig) - EditorConfig support
* [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) - rename tag plugin
* [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) - close tag plugin
* [prettier - code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - prettier code formatter

Nice to have:

* [One Dark Pro](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme) - dark color theme
* [Color Highlight](https://marketplace.visualstudio.com/items?itemName=naumovs.color-highlight) - highlights color in code
* [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) - path import suggestions
* [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense) - import suggestions based on `package.json`
* [filesize](https://marketplace.visualstudio.com/items?itemName=mkxml.vscode-filesize) - file size info in the status bar of the editor
* [gitlens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) - git supercharged
* [import cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost) - display imported package size
* [node readme](https://marketplace.visualstudio.com/items?itemName=bengreenier.vscode-node-readme) - readme file preview
* [reactjs code snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.ReactSnippets) - code snippets for react development

### Snippets

* [snippets.javascript.json](snippets.javascript.json)

### EditorConfig

* [.editorconfig](.editorconfig)
