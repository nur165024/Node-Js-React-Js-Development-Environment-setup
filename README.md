<p align="center">
    <img width="100px" src="image/JavaScript.png" />
    <h1 align="center">Javascript Development Environment Setup</h1>
</p>

## Table of Contents (VS Code)

- [VS Code Extensions](#vs-code-extensions)
- [VS Code Global settings](#vs-code-global-settings)
- [React Js](#react-js)
  - [Settings command line](#settings-command-line)
  - [Workspace Settings](#workspace-settings)
  - [Eslintrc Settings](#eslintrc-settings)
- [Node Js](#node-js)
  - [Node Js Settings command line](#node-js-settings-command-line)
  - [Node Js Workspace Settings](#node-js-workspace-settings)
  - [Node Js Eslintrc Settings](#node-js-eslintrc-settings)

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
- [Typescript React code snippets]
- [Auto Rename Tag]
- [Thunder Client as like postman]

### VS Code Global settings

```json
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
  "workbench.colorTheme": "Learn with Sumit - Peace of the eye",
  "editor.tabSize": 2
}
```

## React Js

React js command line, workspace & Eslintrc settings follow the bellow :

### Settings command line

#### Install Dev Dependencies

```sh
  npm install -D prettier
  npm install -D babel-eslint
  npx install-peerdeps --dev eslint-config-airbnb
  npm install -D eslint-config-prettier eslint-plugin-prettier
```

OR You can also add a new script in the scripts section like below to install everything with a single command:

```json
scripts: {
  "lint": "npm install -D prettier && npm install -D babel-eslint && npx install-peerdeps --dev eslint-config-airbnb && npm install -D eslint-config-prettier eslint-plugin-prettier"
}
```

and then simply run the below command in the terminal -

```sh
  npm run lint
```

### Workspace Settings

```json
{
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
  "javascript.validate.enable": false, //disable all built-in syntax checking
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.fixAll.tslint": true,
    "source.organizeImports": true
  },
  "eslint.alwaysShowStatus": true,
  // emmet
  "emmet.triggerExpansionOnTab": true,
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  }
}
```

### Eslintrc Settings

Create a `.eslintrc.json` file in the project root and enter the below contents:

```json
{
  "extends": [
    "airbnb",
    "airbnb/hooks",
    "eslint:recommended",
    "prettier",
    "plugin:jsx-a11y/recommended"
  ],
  "parser": "babel-eslint",
  "parserOptions": {
    "ecmaVersion": 8
  },
  "env": {
    "browser": true,
    "node": true,
    "es6": true,
    "jest": true
  },
  "rules": {
    "react/react-in-jsx-scope": 0,
    "react-hooks/rules-of-hooks": "error",
    "no-console": 0,
    "react/state-in-constructor": 0,
    "indent": 0,
    "linebreak-style": 0,
    "react/prop-types": 0,
    "jsx-a11y/click-events-have-key-events": 0,
    "react/jsx-filename-extension": [
      1,
      {
        "extensions": [".js", ".jsx"]
      }
    ],
    "prettier/prettier": [
      "error",
      {
        "trailingComma": "es5",
        "singleQuote": true,
        "printWidth": 100,
        "tabWidth": 4,
        "semi": true,
        "endOfLine": "auto"
      }
    ]
  },
  "plugins": ["prettier", "react", "react-hooks"]
}
```

## Node Js

Node js command line, workspace & Eslintrc settings follow the bellow :

### Node Js Settings command line

#### Install Dev Dependencies

```sh
  npm install -D eslint prettier
  npx install-peerdeps --dev eslint-config-airbnb-base
  npm install -D eslint-config-prettier eslint-plugin-prettier
```

### Node Js Workspace Settings

```json
{
  // config related to code formatting
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "[javascript]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.organizeImports": true
  },
  "eslint.alwaysShowStatus": true
}
```

### Node Js Eslintrc Settings

Create a `.eslintrc.json` file in the project root and enter the below contents:

```json
{
  "extends": ["prettier", "airbnb-base"],
  "parserOptions": {
    "ecmaVersion": 12
  },
  "env": {
    "commonjs": true,
    "node": true
  },
  "rules": {
    "no-console": 0,
    "indent": 0,
    "linebreak-style": 0,
    "prettier/prettier": [
      "error",
      {
        "trailingComma": "es5",
        "singleQuote": true,
        "printWidth": 100,
        "tabWidth": 4,
        "semi": true
      }
    ]
  },
  "plugins": ["prettier"]
}
```
