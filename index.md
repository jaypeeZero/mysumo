---
layout: default
title: Home
---

# Recent Posts

{% for post in site.myposts %}
* [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
