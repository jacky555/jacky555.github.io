---
layout: post
title: 网页设计中内容错位的原因及解决办法
category: web-desing
---

今天在做一个小网站的时候，发现有两个页面在观看的时候，会有错位的感觉。这里说的错位就是说：A页面距离显示器左边有100个像素，而切换到B页面以后，反而给人感觉距离显示器左边只有92个像素。

查了这两个页面的标签，没有不对称标签，也没有不符合规则的标签。这是怎么回事呢？

在我观察这两个页面的时候，发现好像就是因为B页面多了一个滚动条的原因造成的这个现象。我把A页面的内容也撑到一屏多，再观察这两个页面，发现OK了。可以肯定是由于滚动条的出现，而导致了这个情况的出现。

在明白了原因以后，解决办法就好说了。

1、把A页面的内容撑到一屏以上。这个办法还是有不科学的。

2、在在样式表中添加html{overflow-y:scroll;}，强制页面出现滚动条。这个办法相比以上，还是有一定科学性的，不过也会因此而出现滚动条了。

两种办法，各有优劣。具体情况，具体分析吧。
