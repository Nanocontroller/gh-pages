---
layout : "default"
title: Design
---

This is theproject called: {{design.title}}
Which belongs to my {{{summary}}}
{{{design.description}}}

<ul>
{{# design.all }}
  <li>
    <a href="{{url}}">{{title}}</a>
    {{{ summary }}}
  </li>
{{/ design.all }}
</ul>