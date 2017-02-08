---
title: 'Third Design'
date: '2017-02-05'
categories: design
description:
tags: []
layout : "docs-layout"
---

In order to create valid [HTML], you need properly
coded syntax that can be cumbersome for 
"non-programmers" to write. Sometimes, you just want
to easily make certain words **bold**, and certain 
words *italicized* without having to remember the 
syntax. Additionally, for example, creating lists:

* should be easy
* should not involve programming

[HTML]: http://en.wikipedia.org/wiki/HTML
<iframe width="560" height="315" src="https://www.youtube.com/embed/boKRYxwZyKw" frameborder="0" allowfullscreen></iframe>



{{# projects.next }}
  Next: <a href="{{ url }}">{{ title }}</a></li>
{{/ projects.next }}

{{# projects.previous }}
  Previous: <a href="{{ url }}">{{ title }}</a></li>
{{/ projects.previous }}