---
title: 'HelioRoom'
categories: ['research/embedded-phenomena', 'HCI']
date: 
description:
tags: [tag1, tag2, tag3]
content: "blah blah blah.........."
layout : posts
---
<!-- <img src="{{urls.media}}/Project.{{page.title}}.png"> -->
![HelioRoom setup]({{urls.media}}/Project.{{page.title}}.png "HelioRoom")


>HelioRoom is a simulation of the solar system, adopting the idea of that the center of the classroom is mapped to the center of the sun. Computer screens attached to each wall of the classroom become observation portals “view-ports” where the planets can be observed in the outer space. As the planets orbit around the Sun, they pass through the view-ports, and temporarily disappear as they travel through interstices between displays, then reappear in the next view-port, along a counter-clockwise path.

<div class="content">
HelioRoom is intended for use in lower elementary grades as a follow-on activity to an introductory unit on the Solar system. The typical content of such units includes the principle of heliocentrism, along with the order, size, and orbital periods of the planets. Ordinarily, this represents "tacit" knowledge for young learners: a set of facts without immediate applicability. HelioRoom is designed to provide an environment within which new knowledge about the order and relative orbital periods of the planets may be reinforced by applying it in a problem-solving context
In support of those learning goals, HelioRoom takes several liberties. The planets are presumed to orbit along strictly planar, circular paths. The depiction of the planets as they pass through the view-ports ignores visual differences owing to distances, size, or surface features; circles of same sizes and different colors represent the planets. (Common color associations, e.g., red Mars or green Earth, were intentionally avoided.) The orbital periods of the planets are shortened, but proportional consistency is maintained.
The instructional challenge to the students is to determine which color has been used to represent each planet. In order to accomplish this task, they must utilize information gathered from observations within two evidentiary systems; the relative order of the planets as indicated by occlusions as one planet passes in front of another, and the relative orbital speeds of the planets. Students gather their data using a tablet that updates the state of the data in real time, so they can discuss their results and draw conclusions as a group.
</div>
<hr>

<div class="summary">
  Quick Summary of HelioRoom post!
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