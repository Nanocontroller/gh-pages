---
layout : "default"
---

{{# projects.paginator }}
<div class="post">
  <h3 class="title"><a href="{{url}}">{{title}}</a></h3>

  {{{ summary }}}

  <div class="more">
    <a href="{{url}}" class="btn btn-small">read more..</a>
  </div>
</div>
{{/ projects.paginator }}

<div class="pagination">
  <ul>
  {{#projects.paginator_navigation}}
    {{#is_active_page}}
      <li class="active"><a href="{{url}}">{{name}}</a></li>
    {{/is_active_page}}
    {{^is_active_page}}
      <li><a href="{{url}}">{{name}}</a></li>
    {{/is_active_page}}
  {{/projects.paginator_navigation}}
  </ul>
</div>
