---
title: "params.toml"
date: 2020-10-19T05:12:05+09:00
draft: false
weight: 5
---

此文件中的参数仅在 zdoc 主题中使用。

### logo

是否要在导航栏中使用 logo icon。

```>:params.toml
logo = true
```

{{< expand "logo" >}}
![Zdoc theme param - logoText](/images/configuration/zdoc/params.toml/1.logo.png)
{{< /expand >}}

### logoText

Logo 文本出现在导航栏中。

```>:params.toml
logoText = "安邦的博客"
```

{{< expand "logoText" >}}
![Zdoc theme param - logoText](/images/configuration/zdoc/params.toml/2.logoText.png)
{{< /expand >}}

### logoType

- short: default. 将 logo 视为正方形。
- long: 将 logo 视为矩形。

```>:params.toml
logoType = "short"
```

{{< expand "logoType" >}}
![Zdoc theme param - logoType](/images/configuration/zdoc/params.toml/1.logo.png)
{{< /expand >}}

### description

用于搜索引擎优化（SEO）

```>:params.toml
description = "My Awesome Blog!"
```

### useFaviconGenerator

是否要使用 [favicon-generator](https://www.favicon-generator.org/)。 如果您想将此参数设置为 true，请参阅 [Favicon](/zzo/userguide/favicon)。

```>:params.toml
useFaviconGenerator = true
```

{{< expand "useFaviconGenerator" >}}
![Zdoc theme param - useFaviconGenerator](/images/configuration/zdoc/params.toml/3.favicon.png)
{{< /expand >}}

### wideViewAsDefault

Set it true when you want a wide page view. If true, TOC or menu sidebar will be folded as default.

当您想要一个宽页面视图时将其设置为 true。 如果为 true，TOC 或菜单侧边栏将默认折叠。

```>:params.toml
wideViewAsDefault = true
```

{{< expand "wideViewAsDefault" >}}

- `true`
  ![Zdoc theme param - wideViewAsDefault](/images/configuration/zdoc/params.toml/4.wideview-1.png)
- `false`
  ![Zdoc theme param - wideViewAsDefault](/images/configuration/zdoc/params.toml/4.wideview-2.png)
  {{< /expand >}}

### enableWideBlogSwitch

当为 true 时，一个视口大小切换按钮将出现在博客文章页面上。

```>:params.toml
enableWideBlogSwitch = true
```

{{< expand "enableWideBlogSwitch" >}}
![Zdoc theme param - enableWideBlogSwitch](/images/configuration/zdoc/params.toml/5.wideblogswitch.png)
{{< /expand >}}

### enableTocSwitch

当为 true 时，一个 toc-visibility 切换按钮将出现在博客文章页面上。

```>:params.toml
enableTocSwitch = true
```

{{< expand "enableTocSwitch" >}}
![Zdoc theme param - enableTocSwitch](/images/configuration/zdoc/params.toml/6.tocswitch.png)
{{< /expand >}}

### enableSearch

如果要启用搜索功能，请设置为 true。

```>:params.toml
enableSearch = true
```

{{< expand "enableSearch" >}}
![Zdoc theme param - enableSearch](/images/configuration/zdoc/params.toml/7.enableSearch.png)
{{< /expand >}}

### enableSearchHighlight

当为 true 时，搜索文本将被着色。

```>:params.toml
enableSearchHighlight = true
```

{{< expand "enableSearchHighlight" >}}
![Zdoc theme param - enableSearchHighlight](/images/configuration/zdoc/params.toml/8.enableSearchHighlight.png)
{{< /expand >}}

### enableLangChange

```>:params.toml
enableLangChange = true
```

{{< expand "enableLangChange" >}}
![Zdoc theme param - enableLangChange](/images/configuration/zdoc/params.toml/9.enableLangChange.png)
{{< /expand >}}

### enableDarkMode

当为 true 时，导航栏上将出现一个主题切换按钮。

```>:params.toml
enableDarkMode = true
```

{{< expand "enableDarkMode" >}}
![Zdoc theme param - enableDarkMode](/images/configuration/zdoc/params.toml/10.enableDarkMode.png)
{{< /expand >}}

### enableBreadcrumb

当为 false 时，面包屑将在每个文档页面上消失。

```>:params.toml
enableBreadcrumb = true
```

{{< expand "enableBreadcrumb" >}}
![Zdoc theme param - enableBreadcrumb](/images/configuration/zdoc/params.toml/11.enableBreadcrumb.png)
{{< /expand >}}

### enableBlogBreadcrumb

如果为 false，则面包屑会在每篇博文中消失。

```>:params.toml
enableBlogBreadcrumb = true
```

{{< expand "enableBlogBreadcrumb" >}}
![Zdoc theme param - enableBlogBreadcrumb](/images/configuration/zdoc/params.toml/12.enableBlogBreadcrumb.png)
{{< /expand >}}

### enableEditBtn

当为真时，`EDIT THIS PAGE` 按钮将出现在页面上。

```>:params.toml
enableEditBtn = true
```

{{< expand "enableEditBtn" >}}
![Zdoc theme param - enableEditBtn](/images/configuration/zdoc/params.toml/13.enableEditBtn.png)
{{< /expand >}}

### enableToc

隐藏/显示目录 (TOC)。

```>:params.toml
enableToc = true
```

{{< expand "enableToc" >}}
![Zdoc theme param - enableToc](/images/configuration/zdoc/params.toml/14.enableToc.png)
{{< /expand >}}

### enableMenu

隐藏/显示菜单侧边栏。

```>:params.toml
enableMenu = true
```

{{< expand "enableMenu" >}}
![Zdoc theme param - enableMenu](/images/configuration/zdoc/params.toml/15.enableMenu.png)
{{< /expand >}}

### enableNavbar

隐藏/显示导航栏

```>:params.toml
enableNavbar = true
```

{{< expand "enableNavbar" >}}
![Zdoc theme param - enableNavbar](/images/configuration/zdoc/params.toml/16.enableNavbar.png)
{{< /expand >}}

### enableFooter

隐藏/显示页脚

```>:params.toml
enableFooter = true
```

{{< expand "enableFooter" >}}
![Zdoc theme param - enableFooter](/images/configuration/zdoc/params.toml/17.enableFooter.png)
{{< /expand >}}

### showPoweredBy

Hide/Show `poweredBy` text in the footer.

```>:params.toml
showPoweredBy = true
```

{{< expand "showPoweredBy" >}}
![Zdoc theme param - showPoweredBy](/images/configuration/zdoc/params.toml/18.showPoweredBy.png)
{{< /expand >}}

### paginateWindow

Setting it to 1 gives 7 buttons, 2 gives 9, etc. If set 1: [1 ... 4 5 6 ... 356] [1 2 3 4 5 ... 356] etc

将其设置为 1 给出 7 个按钮，2 给出 9 个，依此类推。如果设置为 1: [1 ... 4 5 6 ... 356] [1 2 3 4 5 ... 356] 等

```>:params.toml
paginateWindow = 1
```

### taxoPaginate

博客标签页面上每页的元素数量。

```>:params.toml
taxoPaginate = 5
```

### taxoGroupByDate

- "2006-01": group by month
- "2006": group by year

```>:params.toml
taxoGroupByDate = "2006"
```

### github

导航栏中 GitHub 图标的链接

### enableComment

您可以将评论组件添加到博客类型页面。 支持的评论服务是

- utterances
