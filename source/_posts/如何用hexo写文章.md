---
title: 如何用hexo写文章
date: 2021-07-26 13:12:01
tags:
---
1、用cnpm run server 来启动本地预览，在浏览器输入http://localhost:4000/即可。

2、打开terminal，在命令行输入：

hexo new "article" # 文章标题

执行后会在_posts里看见多了一个article.md文件。
刷新页面（http://localhost:4000/）我们能看见新添一个名字叫"文章标题"的文章，没有任何内容。
而这个_posts文件夹，算是一个比较特殊的文件夹，因为它装着所有你发布出去的文章。

打开article.md文件，我们会看到

---
title: 1
date: 2017-09-15 19:00:41
tags:
---
在这里随便写点什么
然后刷新页面,就会看到你写的内容。与此同时，hexo也会自动为这个post生成一个页面，当我们点击标题，就会进入那个页面。


3、草稿箱

打开terminal，在命令行输入：

hexo new draft b

我们会在source下看见一个新的文件夹，_drafts，这个里面会装我们所有的草稿文件。

那写好了的草稿，如何可以在不发布的情况下，预览一下文章在网站上的样子呢？

hexo server --draft

4: 发布草稿

hexo publish b

你会发现_drafts里的b.md不见了，跑到了_posts里面,也就说明你的草稿发布成功了。

........