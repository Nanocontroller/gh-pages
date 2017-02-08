---
title: 'WallCology'
categories: "research/embedded-phenomena"
date: '2017-02-03'
description: 'some description'
tags: [research, implementation, design]
layout : posts
---
#For some reason I think *{{page.title}}* should have this header.


Some of these words *are emphasized*.
Some of these words _are emphasized also_.

Use two asterisks for **strong emphasis**.
Or, if you prefer, __use two underscores instead__.

<img src="{{urls.media}}/Project.{{page.title}}.png">

----------------------------
<div class="summary">
  Quick Summary of my WallCology post!
</div>
----------------------------

<ul class="tag_box inline">
      <li><i class="icon-folder-open"></i></li>
    {{# projects.all }}
      {{> categories_list }}
    {{/ projects.all }}
    </ul>
----------------------------


<ul class="tag_box inline">

{{# projects.next }}
  Next:<li> <i class="icon-folder-open"><a href="{{ url }}">{{ title }}</a></li>
{{/ projects.next }}

{{# projects.previous }}
  Previous: <li><a href="{{ url }}">{{ title }}</a></li>
{{/ projects.previous }}

<ul>
{{# projects.all }}
  {{# is_active_page }}
    <li class="active"><a href="{{ url }}" class="active">{{ title }}</a></li>
  {{/ is_active_page }}
  {{^ is_active_page }}
    <li><a href="{{ url }}">{{ title }}</a></li>
  {{/ is_active_page }}
{{/ projects.all }}
  </ul>