---
layout: page
title: Home
id: home
permalink: /
---

[[About]] [[Publications]] [[Projects]] [[Blog]]
# Welcome! 🌱

Hi There! I’m currently a rising sophomore undergraduate at Cornell University, studying Mathematics and Computer Science and focusing on computer graphics and vision.
Find more about me here: [[About]]


<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
