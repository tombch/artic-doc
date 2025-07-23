---
title: MeV (Measles virus)
tname: MeV<br>(Measles virus)
keywords: resources
summary: A collection of resources for whole genome sequencing and analysis of Measles virus (MeV)
image: /images/viruses/mev.png
sidebar: artic_sidebar
permalink: /viruses/mev
icon: /images/viruses/mev_icon.svg
folder: viruses
tags: [resources, viruses]
---

> A collection of resources for whole genome sequencing and analysis of Measles virus (EBOV)

## Resources and documents

{% assign docs = site.html_pages | where_exp:"item", "item.category contains 'mev'" | sort: 'title' %}
<ul>
{% for doc in docs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

### Setup guides
{% assign mevDocs = site.html_pages | where_exp:"item", "item.category contains 'mev-it-setup'" | sort: 'title' %}
<ul>
{% for doc in mevDocs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

### User-interface pipelines using Epi2me
{% assign mevDocs = site.html_pages | where_exp:"item", "item.category contains 'mev-epi2me'" | sort: 'title' %}
<ul>
{% for doc in mevDocs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

### Command line interface pipeline SOPs
{% assign mevDocs = site.html_pages | where_exp:"item", "item.category contains 'mev-cli'" | sort: 'title' %}
<ul>
{% for doc in mevDocs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

{% include links.html %}
