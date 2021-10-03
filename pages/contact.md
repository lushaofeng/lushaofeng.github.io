---
layout: page
permalink: /contact/
title: Contact
show_meta: false
published: true
description: "Contact information"
comments: false
mathjax: false
noindex: false
sitemap:
    priority: 0.5
    changefreq: 'monthly'
    lastmod: 2016-02-13
tags:
  - "Lu Shaofeng"
  - "driving directions"
  - address
---

<!-- 
| <i class="fa fa-twitter"></i> | [@{{ site.owner.twitter }}](https://twitter.com/{{ site.owner.twitter }})  | 
| - | :- | -->


| <i class="fa fa-map-marker"></i> | Lu Shaofeng <br>South China University of Technology<br>777 Fuxing Ave East, Panyu District<br> Guangzhou 215000| 
| - | :- |
| <i class="fa fa-envelope" aria-hidden="true"></i> | shaofeng.lu_at_hotmail.com (private) <br> lushaofeng_at_scut.edu.cn(work)| 
| - | :- |
| <i class="fa fa-phone" aria-hidden="true"></i> | +86(0)20-81182116 (work)| 
| - | :- |

<a href="https://twitter.com/share" class="twitter-share-button" data-via="{{ site.owner.twitter }}" data-size="small" data-dnt="true">Tweet</a> <a href="javascript:window.print()" class="social-icons" title="Printer friendly format"><i class="fa fa-print"></i></a>

<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+'://platform.twitter.com/widgets.js';fjs.parentNode.insertBefore(js,fjs);}}(document, 'script', 'twitter-wjs');</script>

{% if site.twitter_widget_id %}
<div class="text-tweets">
<div class="tweets">
<a class="twitter-timeline"
  data-dnt="true"
  width="600"
  height="250"
  href="https://twitter.com/{{ site.owner.twitter }}"
  data-widget-id="{{ site.twitter_widget_id }}"
  data-tweet-limit="2"
  data-chrome="noheader nofooter noborders noscrollbar transparent">
  Recent Tweets</a>
 </div>
<script>
    !function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");
</script>
</div>
{% else %}

{% comment %}
Twitter stream will show up here if `twitter_widget_id` is present is `_config.yml

<a class="twitter-timeline" href="https://twitter.com/ShaofengLu1?ref_src=twsrc%5Etfw">Tweets by ShaofengLu1</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

{%endcomment%}
{% endif %}
