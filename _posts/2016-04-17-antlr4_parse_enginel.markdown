---
layout:     post
title:      "Base antlr4 framework,build DSL engine"
subtitle:   "Base antlr4 framework,build DSL engine"
date:       2016-04-17 10:00:00
author:     "Young"
header-img: "img/post-bg-01.jpg"
---
<h2 class="section-heading">Base antlr4 framework,build DSL engine</h2>

<p>基于antlr4，编写一个dsl的引擎</p>

<p><a href="https://github.com/IBYoung/gateway_dsl.git">DSL</a></p>

<h2 class="section-heading">micro server</h2>

<p>设计gateway的时候，我就发现路由的规则，会经常发生变化，比如有时候对接业务，今天想要连接的是这个微服务，明天因为版本升级需要切换，如果假设硬编写代码可以完成，但是需要
额外的升级gateway，这个就给我带来非常大的成本；另一方面，分发的规则，docker的container的伸缩性，我们想要不同节点接受，所以想要引入DSL的语法，能够
借助更多人的帮助，帮我们的gateway更加健壮性，比如数据分析师、运维工程师等，使用一套大家都能够接受的简单语法，然后通过解释器去形成规则。</p>

<a href="#">
    <img src="{{ site.baseurl }}/img/post-sample-image.jpg" alt="Post Sample Image">
</a>
<span class="caption text-muted">To go places and do things that have never been done before – that’s what living is all about.</span>

<p>Space, the final frontier. These are the voyages of the Starship Enterprise. Its five-year mission: to explore strange new worlds, to seek out new life and new civilizations, to boldly go where no man has gone before.</p>

<p>As I stand out here in the wonders of the unknown at Hadley, I sort of realize there’s a fundamental truth to our nature, Man must explore, and this is exploration at its greatest.</p>

<p>Placeholder text by <a href="http://spaceipsum.com/">Space Ipsum</a>. Photographs by <a href="https://www.flickr.com/photos/nasacommons/">NASA on The Commons</a>.</p>

