---
tname: MPXV<br>(mpox virus)
title: MPXV (mpox virus)
keywords: resources
summary: A collection of resources for whole genome sequencing and analysis of MPXV
image: /images/viruses/mpxv.png
sidebar: artic_sidebar
permalink: /viruses/mpxv
icon: /images/viruses/mpxv_icon.svg

folder: viruses
tags: [resources, viruses]
---

> A collection of resources and documents for the genome sequencing of Mpox virus (MPXV) using a tiled amplicon approach.

## Resources and documents

{% assign mpxvDocs = site.html_pages | where_exp:"item", "item.category contains 'mpxv-guide'" | sort: 'title' %}
<ul>
{% for doc in mpxvDocs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

### Setup guides
{% assign mpxvDocs = site.html_pages | where_exp:"item", "item.category contains 'mpxv-setup'" | sort: 'title' %}
<ul>
{% for doc in mpxvDocs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

### User-interface pipelines using Epi2me
{% assign mpxvDocs = site.html_pages | where_exp:"item", "item.category contains 'mpxv-epi2me'" | sort: 'title' %}
<ul>
{% for doc in mpxvDocs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

### Command line interface pipeline SOPs
{% assign mpxvDocs = site.html_pages | where_exp:"item", "item.category contains 'mpxv-cli'" | sort: 'title' %}
<ul>
{% for doc in mpxvDocs %}
    <li>{{ doc.title_text }}</li>
	<blockquote>link: <a href="{{ doc.permalink }}">{{ doc.permalink }}</a></blockquote>
{% endfor %}
</ul>

{% include links.html %}
