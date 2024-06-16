---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: Pulse sequences
permalink: /sequences/
---

{% assign sequences = site.data.projects | where: "type", "sequence" %}

<div class="container">
    {% for project in sequences %}
        {% include project.html %}
    {% endfor %}
</div>

