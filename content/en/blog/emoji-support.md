+++
author = "朱安邦"
title = "本主题支持Emoji"
date = "2019-03-05"
description = "这是本篇文章的Description"
tags = [
    "emoji",
]
+++

Emoji 表情符号可以通过多种方式在 Hugo 项目中启用。

<!--more-->

[`emojify`](https://gohugo.io/functions/emojify/) 函数可以直接在模板或 [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes) 中调用。

To enable emoji globally, set `enableEmoji` to `true` in your site’s [configuration](https://gohugo.io/getting-started/configuration/) and then you can type emoji shorthand codes directly in content files; e.g.

要全局启用表情符号，请在站点配置中将 `enableEmoji` 设置为 `true` ，然后您可以直接在 [configuration](https://gohugo.io/getting-started/configuration/) 文件中键入表情符号简写代码；例如 🙈

<p>
<span class="nowrap">
	<span class="emojify">🙈</span> 
	<code>:see_no_evil:</code>
</span>

<span class="nowrap">
	<span class="emojify">🙉</span> 
	<code>:hear_no_evil:</code>
</span>

<span class="nowrap">
	<span class="emojify">🙊</span> 
	<code>:speak_no_evil:</code>
</span>
</p>
<br>

[Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) 是表情符号速记代码的有用参考。

---

**N.B.** 上述步骤在 Hugo 中启用了 Unicode 标准表情符号字符和序列，但是这些字形的呈现取决于浏览器和平台。 要设置表情符号的样式，您可以使用第三方表情符号字体或字体堆栈； 例如

{{< highlight html >}}
.emoji {
	font-family: Apple Color Emoji,Segoe UI Emoji,NotoColorEmoji,Segoe UI Symbol,Android Emoji,EmojiSymbols;
}
{{< /highlight >}}

{{< css.inline >}}

<style>
.emojify {
	font-family: Apple Color Emoji,Segoe UI Emoji,NotoColorEmoji,Segoe UI Symbol,Android Emoji,EmojiSymbols;
	font-size: 2rem;
	vertical-align: middle;
}
@media screen and (max-width:650px) {
    .nowrap {
	display: block;
	margin: 25px 0;
}
}
</style>

{{< /css.inline >}}
