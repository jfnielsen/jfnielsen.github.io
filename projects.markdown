---
layout: page
title: Projects
permalink: /projects/
---

{% assign tools = site.data.projects | where: "type", "tool" %} 
{% assign sequences = site.data.projects | where: "type", "sequence" %}
{% assign allprojects = site.data.projects %} 

<h2> Development tools </h2>
<div class="container">
    {% for project in tools %}
        {% include project.html %}
    {% endfor %}
</div>

<br>
<br>
<h2> Pulse sequences </h2>
<div class="container">
    {% for project in sequences %}
        {% include project.html %}
    {% endfor %}
</div>

