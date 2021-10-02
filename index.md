---
layout: default
permalink: index.html
title: Personal Homepage of Lu Shaofeng 
description: "Blogging on ...."
---

Hi, my name is Lu Shaofeng. I am currently an Associate Professor with the Shien-Ming Wu School of Intelligent Engineering, South China University of Technology (SCUT). Before joining SCUT, I was a faculty member with Department of Electrical and Electronic Engineering, Xi'an Jiaotong-Liverpool University (XJTLU) from Sep. 2013 to Aug. 2019.

My research interests include railway traction systems, renewable power systems, meta-heuristic and numerical optimisation techniques, electric and hybrid driving systems, electric networks, power management strategies, energy storage devices and complex network. <a href="/about/">Read more about my professional life story...</a>

<div class="posts">
  {% for post in site.categories.featured limit:2 %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ site.url }}{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

  {% if post.modified.size > 2 %}<span class="post-date indexpg" itemprop="dateModified" content="{{ post.modified | date: "%Y-%m-%d" }}">
    <i class="fa fa-edit" title="Last updated"> {{ post.modified | date_to_string }}</i> 
    <a href="{{ site.url }}/featured" title="Featured posts"><i class="fa fa-paperclip" title="Featured" class="social-icons"></i></a></span>{% else %}<span class="post-date indexpg" itemprop="datePublished" content="{{ post.date | date: "%Y-%m-%d" }}">
    <i class="fa fa-calendar" title="Date published"> {{ post.date | date_to_string }}</i> 
    <a href="{{ site.url }}/featured" title="Featured posts"><i class="fa fa-paperclip" title="Featured" class="social-icons"></i></a></span>{% endif %}

 {% if post.description.size > 140 %}{{ post.description | markdownify | remove: '<p>' | remove: '</p>' }}{% else %}{{ post.excerpt | markdownify | remove: '<p>' | remove: '</p>' }}{% endif %} <a href="{{ site.url }}{{ post.url }}" title="Read more"><strong>Read more...</strong></a>
  </div>
  <hr class="transp">
  {% endfor %}
</div>

<div class="posts">
  {% for post in site.posts limit:2 %}
  {% unless post.category contains "featured" %} 
  <div class="post">
    <h1 class="post-title">
      <a href="{{ site.url }}{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

  {% if post.modified.size > 2 %}<span class="post-date indexpg" itemprop="dateModified" content="{{ post.modified | date: "%Y-%m-%d" }}"><i class="fa fa-edit" title="Last updated"> {{ post.modified | date_to_string }}</i></span>{% else %}<span class="post-date indexpg" itemprop="datePublished" content="{{ post.date | date: "%Y-%m-%d" }}"><i class="fa fa-calendar" title="Date published"> {{ post.date | date_to_string }}</i></span>{% endif %}

 {% if post.description.size > 140 %}{{ post.description | markdownify | remove: '<p>' | remove: '</p>' }}{% else %}{{ post.excerpt | markdownify | remove: '<p>' | remove: '</p>' }}{% endif %} <a href="{{ site.url }}{{ post.url }}" title="Read more"><strong>Read more...</strong></a>
  </div>
  {% unless forloop.last %}<hr class="transp">{% endunless %}
  {% endunless %}
  {% endfor %}
</div>

<h3 class="post-title">
<div class="pagination" style="margin: 0.5rem;">
    <a class="pagination-item older" href="{{ site.url }}/blog"><i class="fa fa-edit"> Blog</i></a>
    <a class="pagination-item newer" href="{{ site.url }}/tags"><i class="fa fa-tags"> Tags</i></a>
</div>
</h3>
