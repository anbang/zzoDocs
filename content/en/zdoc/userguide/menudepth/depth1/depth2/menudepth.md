---
title: "菜单深度"
date: 2020-10-21T06:24:22+09:00
draft: false
weight: 2
enableToc: false
---

## 深度文件夹结构

```
userguide
├── Depth - 1
│   ├── _index.md
│   ├── Depth - 2
│   │   ├── _index.md
│   │   ├── Depth - 3
│   │   │   ├── _index.md
│   │   │   ├── menudepth.md
```

## 如何使菜单可折叠。

从上面的文件夹结构可以看出，每个可折叠的根文件夹都有一个 `_index.md` 文件。 在该文件中，我们将菜单定义为可折叠的。 如果您希望菜单可折叠，请将 `collapsible` Front-Matter 设置为 true。

```_index.md {hl_lines=[7]}
---
title: "Depth - 3"
date: 2020-02-28T10:08:56+09:00
description:
draft: false
weight: 1
collapsible: true
---
```
