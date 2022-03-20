---
title: "安装"
date: 2020-01-30T00:38:25+09:00
description: Installation description
draft: false
weight: 1
---

## Step 1: 安装 Hugo

本指南假定您已经安装了 [Hugo-extended](https://gohugo.io/getting-started/installing/) 版本 。

## Step 2: 创建新网站

通过键入如下命令创建一个新站点。 它将创建一些空文件夹。 我将在本指南中创建一个 `mydocs` 文件夹。

```
hugo new site mydocs
```

## Step 3: 添加一个主题

您可以从 Github 手动下载并解压主题，但使用 git 克隆 repo 更容易。

```
cd mydocs
git init
git clone https://github.com/zzossig/hugo-theme-zdoc.git themes/zdoc
```

如果您使用 git 对您的站点进行版本控制，强烈推荐，最好将 zdoc 主题添加为子模块。
转到您的站点根文件夹（在我的情况下为 `mydocs` 文件夹）并键入以下内容。

```
cd mydocs
git init
git submodule add https://github.com/zzossig/hugo-theme-zzo.git themes/zdoc
```

## Step 4: 添加 Config 文件

我们必须制作 4 个配置文件才能使主题正常工作。 查看 [配置文件](/zdoc/configuration/configfiles/) 部分。

- [config.toml] - 我们可以设置 Hugo 本身相关的配置参数。
- [languages.toml] - 我们可以更改语言相关设置。
- [menus.en.toml] - 我们可以添加或删除站点菜单。
- [params.toml] - 此文件中的参数仅用于 zdoc 主题。

如果您的博客计划支持多种语言，我建议您先创建一个 contry 代码文件夹，如 [en]、[ko]、[fr] 等。

这样，您可以更有效地管理您的内容。 然后您应该在 `language.toml` 文件中指定内容文件夹。

```:language.toml
[en]
  ...
  contentdir = "content/en"
  ...
```

通过制作 `menus.en.toml` 文件来创建您的站点菜单。 `en` 可以是任何国家代码。 我将在本指南中制作一个文档菜单。

```:menus.en.toml
[[main]]
  identifier = "docs"
  name = "Docs"
  url = "docs"
  weight = 1
  ...
```

## Step 5: 添加一些内容

我将在 `root/content/en` 文件夹中创建 `docs` 文件夹。 菜单的根文件夹应该有 `_index.md` 文件。

```:/content/en/docs/_index.md
---
title: "docs section"
date: 2019-03-26T08:47:11+01:00
description: All the list of my documentation
---
```

上面用于 SEO（搜索引擎优化）的参数(title, date, description)。 我们称参数为 front-matter。 一些 front-matter 用于 SEO，另一些用于显示内容、配置等。现在，让我们制作第一个 markdown 文件。 在 docs 文件夹中制作 md 文件

```:/content/en/docs/myfirstdoc.md
---
title: "My First Document"
date: 2019-03-26T08:47:11+01:00
description: You will find some of the most common and helpful pages from our documentation.
draft: false
---

Your markdown here.
```

## 更新

从您网站的根目录：

```
git submodule update --remote --merge
```

## 运行示例站点

From the root of themes/zdoc/exampleSite:

```
hugo server --themesDir ../..
```
