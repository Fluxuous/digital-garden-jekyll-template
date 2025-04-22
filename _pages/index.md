---
layout: page
title: Home
id: home
permalink: /
---

# Hi, I'm Parker

Welcome to the edge of what’s next.
I write about building the future—from agentic AI and decentralized finance to creative systems, product design, and modern work. If you’re thinking about where tech, capital, and humanity intersect, you’re in the right place.

<strong>Recent Writing</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
