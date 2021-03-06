---
title: 利用 AJAX 刷新部分内容
---

在完成异步搜索功能后（详情看 `search.js`），我在想既然 `json` 格式的数据可以异步加载，那么可以利用该特性对网站的内容进行部分刷新。

异步可以带来很多好处，最显著的是我可以给我的博客添加背景音乐，也就不用担心页面切换的时候背景音乐也被切换。

但是这样带来的后果是，我需要将所有 URL 跳转都变成 AJAX 异步请求，导致 URL 没有变化，这会影响网站的收录，因此我并不打算在文章中使用 AJAX 技术。

但是在首页，当你的文章很多的时候，一口气全部加载出来是不合理的，浏览者并不能一下子看完，因此我需要设计分页功能，当然这个功能是假的，但是实现效果却比真的分页功能强。

当用户点击下一页的时候，后台通过异步加载获得后面的数据，然后将当前页面的内容替换，达到分页的功能，这样页面也不会有卡顿的迹象。

实现思路如下：

1. 服务器端准备相应的 `json` 数据格式，类似 `search.json`，但是不需要全文，只需要文章的标题、地址、时间、标签和摘要等信息。
2. 点击按钮触发 AJAX 请求，然后后台向服务端请求数据。
3. 得到 `json` 数据后拼接相应的 html 模块，然后将原有模块替换，达到换页效果。

本主题当前还未实现，等我有空再来。