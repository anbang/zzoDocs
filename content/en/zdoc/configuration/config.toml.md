---
title: "config.toml"
date: 2020-10-18T17:01:32+09:00
draft: false
weight: 2
---

`config.toml` 文件是 Hugo 本身的配置文件。 所有可能的参数都记录在 [the official Hugo site](https://gohugo.io/getting-started/configuration/#all-configuration-settings)。

### baseURL

将此参数设置为您的站点 URL。 Zdoc 主题正在使用此参数进行搜索。 因此，如果此参数不正确，则搜索将不起作用。 如果您购买了域名，请使用它而不是默认域名。

### theme

要使用的主题（默认位于 /themes/THEMENAME/）。

### defaultContentLanguage

没有语言指示符的内容将默认为此语言。

### defaultContentLanguageInSubdir

在 subdir 中呈现默认的内容语言，例如 `content/en/`。 然后站点根目录`/` 将重定向到`/en/`。

### hasCJKLanguage

如果为真，自动检测内容中的中文/日文/韩文。 这将使 `.Summary` 和 `.WordCount` 对于 CJK 语言的行为正确。

### summaryLength

在 `.Summary` 中显示的文字长度。

### buildFuture

Include content with publishdate in the future.

### copyright

设置您的版权文本。 您可以使用 {year} 打印当前年份。 例如，

```
©{year} zzossig, All Rights Reserved
```

您可以为 [creativecommons](https://creativecommons.org/licenses/by-sa/4.0/)（或任何链接）添加链接。

```
©2018 - {year} All content is licensed under <a target='_blank' rel='external noopener' href='https://example.com'>CC BY-SA</a>
```

### timeout

生成页面内容的超时时间，以毫秒为单位（默认为 10 秒）。 注意：这用于避免递归内容生成，如果您的页面生成速度很慢（例如，因为它们需要大图像处理或依赖于远程内容），您可能需要提高此限制。

### enableEmoji

为页面内容启用 Emoji 表情支持

### paginate

[分页]（https://gohugo.io/templates/pagination/）中每页的默认元素数。

### rssLimit

RSS 提要中的最大项目数。

### enableGitInfo

Enable .GitInfo object for each page (if the Hugo site is versioned by Git). This will then update the Lastmod parameter for each page using the last git commit date for that content file.

### googleAnalytics

谷歌分析跟踪 ID。

### disableKinds

启用禁用指定种类的所有页面。 此列表中允许的值：`"page"`、`"home"`、`"section"`、`"taxonomy"`、`"term"`、`"RSS"`、`"sitemap"`、`" 机器人TXT"`，`"404"`。

### markup

这是一个 markdown 相关的配置。 参见 [official documentation](https://gohugo.io/getting-started/configuration-markup).

### outputs

将此参数用于自定义输出 `SearchIndex`。 如果设置 `home = ["SearchIndex"]`，则可以在 http(s)://www.mydomain.com/index.json 中看到搜索索引。

### outputFormats

用于定义自定义输出`SearchIndex`。 这是一个 json 文件。

### taxonomies

Hugo 支持用户定义的内容分组，称为分类法。 分类法是内容之间逻辑关系的分类。

> Zdoc 官网主题仅使用了 `tag` 分类。
