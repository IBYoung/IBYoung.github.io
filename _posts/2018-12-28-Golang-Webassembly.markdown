---
layout:     post
title:      "Experimental code playing with Go and WebAssembly"
date:       2018-12-28 12:00:00
author:     "CHENYANG"
header-img: "img/post-bg-02.jpg"
---



<p>Welcome All! With Go v1.11 having just been released with an experimental port to WebAssembly included, I thought it would be awesome to see how we can write our own Go programs that compile straight to WebAssembly!</p>

<p>So, in this article, we are going to be building a really simple calculator to give us an idea as to how we can write functions that can be exposed to the frontend, evaluate DOM elements and subsequently update any DOM elements with the results from any functions we call.</p>

<p>This will hopefully show you what it takes to write and compile your own Go-based programs for your frontend applications.</p>

<blockquote>
<p><strong>Note -</strong> If you haven&rsquo;t guessed from the opening line, Go v1.11 will be required in order for this tutorial to work!</p>
</blockquote>

<h1 id="video-tutorial">Video Tutorial</h1>

<p>If you want to support me and my efforts then check out the video version of this tutorial and subscribe to my channel!</p>

<iframe width="560" height="315" src="https://www.youtube.com/embed/4kBvvk2Bzis" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<h1 id="introduction">Introduction</h1>

<p>So what does this really mean for Go and Web developers? Well, it gives us the ability to write our frontend web apps using the Go language and subsequently all its cool features such as its type safety, its <a href="/golang/concurrency-with-golang-goroutines/">goroutines</a> and more.</p>

<p>Now, this isn&rsquo;t the first time we&rsquo;ve seen the Go language being used for frontend purposes. GopherJS has been around for quite a while now and is pretty damn mature, however, the difference is that it compiles Go code to JS and not to WebAssembly.</p>

<h1 id="a-simple-example">A Simple Example</h1>


<p>So what does this really mean for Go and Web developers? Well, it gives us the ability to write our frontend web apps using the Go language and subsequently all its cool features such as its type safety, its <a href="/golang/concurrency-with-golang-goroutines/">goroutines</a> and more.</p>

<p>Now, this isn&rsquo;t the first time we&rsquo;ve seen the Go language being used for frontend purposes. GopherJS has been around for quite a while now and is pretty damn mature, however, the difference is that it compiles Go code to JS and not to WebAssembly.</p>

<h1 id="a-simple-example">A Simple Example</h1>

<a href="http://47.92.237.172:8080/">demo</a>