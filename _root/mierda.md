---
layout : "default"
---

Lorem ipsum dolor sit amet, quam vel ac porta tincidunt eu, sed phasellus cursus quisque sapien turpis, convallis hendrerit. Eros vitae. Pharetra a pede quisquam quam nisl, eu proin quis dictumst sapien, sed vestibulum et ultrices. Integer cras sollicitudin cras, sit mi, metus ultrices dis lorem sodales vitae suscipit, in turpis scelerisque, suspendisse felis porro volutpat vitae dui tincidunt. Arcu ante consequat curabitur penatibus, elit sed sodales velit vivamus, justo pede sit orci lectus pellentesque egestas, dictum ipsum aliquet felis blandit, vestibulum vestibulum dictum placerat. Et commodo, eu proin habitasse id donec neque varius, platea proin, eget purus vitae, neque pede. Ac inceptos mattis arcu integer, tempor sit massa, sociosqu donec id viverra semper, risus non nec in, nec augue nam eros adipiscing est.


<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>{{ page.title }}</title>
    {{# stylesheets.load }}
      style.css
    {{/ stylesheets.load }}
  </head>
  <body>
      <div class="content">
        <p>A cool post about stuff.</p>
        <ul>
          <li>a</li>
          <li>cool</li>
          <li>list</li>
        </ul>
      </div>

      <ul class="tag_box inline">
{{# projects.categories.all }}
  <li>
    Category: <a href="{{ url }}">{{ name }} <span>{{ count }}</span></a>
    <h4>projects</h4>
    <ul>
    {{# projects?to_projects }}
      <li><a href="{{ url }}">{{ title }}</a></li>
    {{/ projects?to_projects }}
    </ul>
  </li>
{{/ projects.categories.all }}
</ul>

  </body>
</html>