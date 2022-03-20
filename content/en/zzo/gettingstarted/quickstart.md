---
title: "快速开始的指南"
date: 2020-01-30T10:16:47+09:00
description:
draft: false
weight: -1
---

如果您不想考虑任何事情，只想获得一个有效的网站，请执行此操作。 本指南假设您已经安装了 [Hugo-extended](https://gohugo.io/getting-started/installing/)

1. 创建一个文件夹作为您网站的根目录。 （例如：c:\\workspace\\mydocs）
2. 转到您在步骤 1 中创建的文件夹目录（在我的情况下为 `mydocs` ），然后通过键入创建一个新的 Hugo 站点

   ```
   hugo new site .
   ```

   请记住，末尾有一个`.`（实际上，`.`表示当前目录）。

3. 下载 [hugo-theme-zdoc](https://github.com/zzossig/hugo-theme-zdoc) 存储库。 我推荐使用 `submodule` ，但这只是一个快速入门指南。 下载存储库比使用 git 子模块更容易。
4. 在您的博客主题文件夹中创建一个“zdoc”文件夹。 （在我的例子中是`mydocs/themes/zdoc`）
5. 解压 zdoc 仓库到你的 zzo 文件夹
6. 在 zdoc 文件夹中，可以看到 exampleSite 文件夹。 里面有四个文件夹（config、content、resources、static）。 只需将它们复制粘贴到您的项目根文件夹即可。 （删除重叠的文件夹或覆盖文件夹）
7. 现在，你可以运行了。 在你的根目录下输入“hugo server”来运行 Hugo。
