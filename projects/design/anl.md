---
title: 'design/anl'
date: '2017-02-05'
description:
tags: []
layout : "default"
---

# My work for ANL
<div class="alert alert-success" role="alert">
  <strong>Well done!</strong> Here is some Argonne stuff.
</div>

Sed ut perspiciatis, unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam eaque ipsa, quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt, explicabo. Nemo enim ipsam voluptatem, quia voluptas sit, aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos, qui ratione voluptatem sequi nesciunt, neque porro quisquam est, qui dolorem ipsum, quia dolor sit amet, consectetur, adipisci[ng] velit, sed quia non numquam [do] eius modi tempora inci[di]dunt, ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit, qui in ea voluptate velit esse, quam nihil molestiae consequatur, vel illum, qui dolorem eum fugiat, quo voluptas nulla pariatur?

----------------------------
<div class="summary">
  Quick Summary of my ANL post!
</div>

<ul class="tag_box inline">

{{# projects.next }}
  Next:<li> <a href="{{ url }}">{{ title }}</a></li>
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