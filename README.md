# vscodeConfig

### 前言

> 一直想写个工具篇的文档，因为有句名话说得好“工欲善其事必先利其器”，如果想要做大事，用好工具我认为还是非常必要的，可以在美观以及代码语法上进行提示（用 vim 或者 txt 文档写代码的大神绕过，求饶命...)。于是乎我这篇文就是这样的存在。主要是针对前端人员最近大家都一起用的 vscode 的插件和配置做一个记录

### 插件

#### 插件名

_（R)： 墙裂推荐_
**美观和格式化用插件**

>

    -Auto Close Tag（R)
    -Auto Import（R)
    -Beautify（R)
    -Prettier（R)
    -Prettify JSON（R)
    -vscode-styled-components（R)

**检测类 插件**

>

    -ESlint（R)
    -Javascript(es6) code snippets

    -Guides
    -IntelliSense for CSS class names in HTML // class name validate
    -Sass

**git 帮助 用插件**

>

    -Git Blame（R)
    -Git History
    -gitignore
    -gitK（R)
    -GitLens（R)

**工具类 开发用插件**

>

    -TODO highlight
    -Coder Runner（R)
    -View In Browser（R)

**vue and react 开发用插件**

>

    -React Redux ES6 Snippets
    -vue 2 snippets
    -vuehelper
    -Vetur

#### 本机安装的插件图片

![vscode plugin img1](http://static.zeroyh.cn/vscode-1.png)
![vscode plugin img2](http://static.zeroyh.cn/vscode-2.png)
![vscode plugin img3](http://static.zeroyh.cn/vscode-3.png)

### vscode setting

```json
{
    "editor.rulers": [120],
    "git.autofetch": true,
    "editor.tabSize": 4,
    "editor.detectIndentation": false,
    "git.enableSmartCommit": true,
    "files.exclude": {
        "**/.git": true,
        "**/.svn": true,
        "**/.hg": true,
        "**/CVS": true,
        "**/.idea": true,
        "**/.DS_Store": true
    },
    "files.eol": "\n",
    "emmet.syntaxProfiles": {
        "vue-html": "html",
        "vue": "html"
    },
    "eslint.enable": true,
    "eslint.validate": [
        "javascriptreact",
        "html",
        {
            "language": "vue",
            "autoFix": true
        },
        {
            "language": "javascript",
            "autoFix": true
        }
    ],
    "vetur.format.options.tabSize": 4,
    "editor.formatOnSave": true,
    // "prettier.eslintIntegration": true,
    "prettier.semi": false,
    "prettier.singleQuote": true,
    "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
    "vetur.validation.template": false,
    "vetur.format.defaultFormatter.html": "js-beautify-html",
    "vetur.format.defaultFormatter.js": "none",
    "vetur.format.defaultFormatterOptions": {
        "js-beautify-html": {
            "wrap_attributes": "force-aligned"
        }
    },
    "editor.wordWrapColumn": 80,
    "prettier.printWidth": 80,
    "prettier.tabWidth": 4,
    "git.confirmSync": false,
    "gitlens.advanced.messages": {
        "suppressShowKeyBindingsNotice": true
    },
    "gitk.fontFamily": "monospace",
    "files.autoSave": "off",
    // "window.menuBarVisibility": "default",
    "window.zoomLevel": 0,
    "editor.fontSize": 16,
    "terminal.integrated.fontSize": 12,
    "search.followSymlinks": false,
    "javascript.updateImportsOnFileMove.enabled": "always",
    "eslint.autoFixOnSave": true,
    "emmet.optimizeStylesheetParsing": false,
    "workbench.activityBar.visible": true,
    "workbench.sideBar.location": "left",
    "guides.enabled": false,
    "explorer.confirmDelete": false,
    "explorer.confirmDragAndDrop": false
}
```
