---
layout: page
title: 安装 Express
description: Learn how to install Express.js in your Node.js environment, including setting up your project directory and managing dependencies with npm.
menu: starter
redirect_from: "  "
---

# 安装

假设您已经安装了 [Node.js](https://nodejs.org/)，创建目录以保存应用程序，并将其设置为工作目录。

- [Express 4.x](/{{ page.lang }}/4x/api.html) requires Node.js 0.10 or higher.
- [Express 5.x](/{{ page.lang }}/5x/api.html) requires Node.js 18 or higher.

```bash
$ mkdir myapp
$ cd myapp
```

使用 `npm init` 命令为应用程序创建 `package.json` 文件。
有关 `package.json` 工作方式的更多信息，请参阅 [Specifics of npm's package.json handling](https://docs.npmjs.com/files/package.json)。

```bash
$ npm init
```

这个命令会要求你输入一些信息，例如应用程序的名称和版本。
目前你只需要按 回车键 接受大多数选项的默认值，只有一项除外：

```
entry point: (index.js)
```

输入 `app.js`，或者您希望使用的任何主文件名称。如果希望文件名为 `index.js`，请按回车键以接受建议的缺省文件名。
在 `myapp` 目录中安装 Express，然后将其保存在依赖项列表中。例如：

```bash
$ npm install express
```

要暂时安装 Express 而不将其添加到依赖项列表中：

```bash
$ npm install express --no-save
```

<div class="doc-box doc-info" markdown="1">

默认情况下，版本为 npm 5.0+ 的 npm install 将模块添加到 `package.json` 文件中的 `dependencies` 列表；对于较早版本的 npm，必须显式指定 `--save` 选项。
今后运行 `app` 目录中的 `npm install` 将自动安装依赖项列表中的模块。

</div>

### [Next: Hello World ](/{{ page.lang }}/starter/hello-world.html)
