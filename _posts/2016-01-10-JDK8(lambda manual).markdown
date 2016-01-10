---
layout:     post
title:      "Lambda Manual"
subtitle:   "Lambda Manual"
date:       2016-01-10 10:00:00
author:     "Young"
header-img: "img/post-bg-01.jpg"
---

<p></p>
<h2 class="section-heading">JDK8 Lambda Manual</h2>

<p>flagmap的功能把多个list整合在一起进行流化</p>
<pre><code class="ruby">
        List<Integer> together = Stream.of(asList(1, 2), asList(3, 4, 5))
                .flatMap(numbers -> numbers.stream())
                .collect(toList());

        assertEquals(asList(1, 2, 3, 4, 5), together);
</code>
</pre>


<p>JDK 8 Lambda manual</p>