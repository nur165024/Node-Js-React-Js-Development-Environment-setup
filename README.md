<p align="center">
    <h3 align="center">Javascript Development Environment Setup</h3>
</p>

## Table of Contents (VS Code)

- [VS code Extensions](#vs-code-extensions)
  - [Global settings](#global-settings)
- [React Js](#react-js)
  - [Settings command line](#ra-js-settings-command-line)
  - [Workspace Settings](#ra-js-workspace-setting)
  - [Eslintrc Settings](#ra-js-eslintrc-settings)
- [Node Js](#react-js)
  - [Settings command line](#node-js-settings-command-line)
  - [Workspace Settings](#node-js-workspace-setting)
  - [Eslintrc Settings](#node-js-eslintrc-settings)

## VS code Extensions

Please follow the below instructions to update node in your machine:

### Extensions

Install the below Extensions :

- [Auto Import]
- [ESLint]
- [JavaScript (ES6) code snippets]
- [Live Server]
- [Learn with sumit color theme]
- [Material Icon Theme]
- [Npm]
- [Npm Intellisense]
- [Path Intellisense]
- [Prettier code Formatter]
- [React Extension Pack]
- [React js code snippets]
- [Search node_modules]

### Global settings

```sh
  {
  // editor
  "editor.fontSize": 18,
  "editor.fontFamily": "Menlo, Monaco,'Courier New',Fira Code",
  "editor.fontLigatures": true,
  "editor.wordWrap": "on",
  "editor.minimap.enabled": false,
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": "comment",
        "settings": {
          "fontStyle": "italic"
        }
      }
    ]
  },
  // cursor
  "editor.cursorSmoothCaretAnimation": true,
  "editor.cursorBlinking": "expand",
  // config related to code formatting
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "[javascriptreact]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.fixAll.tslint": true,
    "source.organizeImports": true
  },
  "eslint.alwaysShowStatus": true,
  //terminal
  "terminal.integrated.fontSize": 16,
  "terminal.integrated.fontWeight": "normal",
  // emmet format html,css,javascript,jsx form emmet
  "emmet.preferences": {},
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "razor": "html",
    "plaintext": "pug"
  },
  // ---------- install vs code extenstion
  // iconTheme theme
  "workbench.iconTheme": "material-icon-theme",
  // live server
  "liveServer.settings.donotVerifyTags": true,
  // color theme
  "workbench.colorTheme": "Learn with Sumit - Peace of the eye"
  }
```

## React Js

React js command line, workspace & Eslintrc settings follow the bellow :

### Settings command line

```sh

```
