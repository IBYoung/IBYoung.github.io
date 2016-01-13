---
layout:     post
title:      "Lambda Manual"
subtitle:   "Lambda Manual"
date:       2016-01-10 10:00:00
author:     "Young"
header-img: "img/post-bg-01.jpg"
---
<h2 class="section-heading">JDK8 Lambda Manual</h2>

<p>flagmap的功能把多个list整合在一起进行流化</p>
<pre><code class="java">
        List together = Stream.of(asList(1, 2), asList(3, 4, 5))
                .flatMap(numbers -> numbers.stream())
                .collect(toList());

        assertEquals(asList(1, 2, 3, 4, 5), together);
        
        
        
         // BEGIN strings_numbers_filter
                List<String> beginningWithNumbers
                        = Stream.of("a", "1abc", "abc1")
                        .filter(value -> isDigit(value.charAt(0)))
                        .collect(toList());
        
                assertEquals(asList("1abc"), beginningWithNumbers);
                // END strings_numbers_filter
</code>
</pre>

