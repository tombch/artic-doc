---
title: "ARTIC network"
keywords: homepage artic
tags: [about]
sidebar: artic_sidebar
permalink: index.html
summary: ARTIC network is a project funded by the Wellcome Trust to develop systems, protocols and bioinformatics for end-to-end pathogen genomics.
toc: false
---

<div class="row">
    <div class="col-lg-12">
        <h2 class="page-header">Sections</h2>
    </div>
    <div class="col-md-3 col-sm-6">
        <div class="panel panel-default text-center">
            <div class="panel-heading">
                <a href="/resources">
                    <span class="fa-stack fa-5x">
                          <i class="fa fa-circle fa-stack-2x text-primary"></i>
                          <i class="fa fa-suitcase fa-stack-1x fa-inverse"></i>
                    </span>
                </a>
            </div>
            <div class="panel-body">
                <h4>Resources</h4>
                <p style="min-height: 75px">Resources, protocols, software and data.</p>
                <a href="/resources" class="btn btn-primary">Learn More</a>
            </div>
        </div>
    </div>
    <div class="col-md-3 col-sm-6">
        <div class="panel panel-default text-center">
            <div class="panel-heading">
                <a href="/documentation">
                <span class="fa-stack fa-5x">
                      <i class="fa fa-circle fa-stack-2x text-primary"></i>
                      <i class="fa fa-book fa-stack-1x fa-inverse"></i>
                </span>
                </a>
            </div>
            <div class="panel-body">
                <h4>Documentation</h4>
                <p style="min-height: 75px">Tutorials, instruction manuals and teaching materials.</p>
                <a href="#" class="btn btn-primary">Learn More</a>
            </div>
        </div>
    </div>
    <div class="col-md-3 col-sm-6">
        <div class="panel panel-default text-center">
            <div class="panel-heading">
                <a href="/projects">
                <span class="fa-stack fa-5x">
                      <i class="fa fa-circle fa-stack-2x text-primary"></i>
                      <i class="fa fa-codepen fa-stack-1x fa-inverse"></i>
                </span>
                </a>
            </div>
            <div class="panel-body">
                <h4>Projects</h4>
                <p style="min-height: 75px">On going and previous projects and collaborations.</p>
                <a href="#" class="btn btn-primary">Learn More</a>
            </div>
        </div>
    </div>
    <div class="col-md-3 col-sm-6">
        <div class="panel panel-default text-center">
            <div class="panel-heading">
                <a href="/people">
                <span class="fa-stack fa-5x">
                      <i class="fa fa-circle fa-stack-2x text-primary"></i>
                      <i class="fa fa-id-badge fa-stack-1x fa-inverse"></i>
                </span>
                </a>
            </div>
            <div class="panel-body">
                <h4>People</h4>
                <p style="min-height: 75px">Network members and collaborators.</p>
                <a href="#" class="btn btn-primary">Learn More</a>
            </div>
        </div>
    </div>
</div>

<hr />

# Latest News
<div class="post-list">
    {% for post in site.posts limit:3 %}
        <h2><a class="post-link" href="{{ post.url | remove: "/" }}">{{ post.title }}</a></h2>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }} /
            {% for tag in post.tags %}
                <a href="{{ "tag_" | append: tag | append: ".html"}}">{{tag}}</a>{% unless forloop.last %}, {% endunless%}

            {% endfor %}
        </span>
        <p>{% if post.summary %} {{ post.summary | strip_html | strip_newlines | truncate: 160 }} {% else %} {{ post.content | truncatewords: 50 | strip_html }} {% endif %}</p>

    {% endfor %}
            
    <br />
    <p><a href="news.html">See more ARTIC News</a>. </p>

</div>

{% include links.html %}
