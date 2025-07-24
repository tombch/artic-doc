---
title: Documentation, tutorials and teaching materials
keywords: training
sidebar: artic_sidebar
toc: true
permalink: /training/tutorials
folder: training
---

## Tutorials

{% assign docs = site.html_pages | where_exp:"item", "item.category contains 'tutorial'" | sort: 'title' %}
<ul>
    {% for doc in docs %}
    <li>{{ doc.title_text }}</li>
    <blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
    {% endfor %}
</ul>



