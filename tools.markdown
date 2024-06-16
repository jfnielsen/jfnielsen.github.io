---
layout: page
title: Software tools
permalink: /tools/
---

{% assign tools = site.data.projects | where: "type", "tool" %}

<div class="container">
    {% for project in tools %}
        {% include project.html %}
    {% endfor %}
</div>

