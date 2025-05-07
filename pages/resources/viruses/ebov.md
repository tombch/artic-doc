---
title: EBOV (Ebola virus) sequencing
keywords: resources
summary: "Resources, primers, protocols and pipelines for sequencing Ebola virus (EBOV)"
image: images/ebov.png
sidebar: resources_sidebar
permalink: ebo
folder: viruses
tags: [resources, viruses]
---

> A collection of resources and documents for the genome sequencing of Ebola virus (EBOV) using a tiled amplicon approach.

## Resources and documents

{% assign docs = site.html_pages | where_exp:"item", "item.category contains 'ebov'" | sort: 'title' %}
<ul>
{% for doc in docs %}
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
