---
layout: post
title: "January 2025 Wrestlers"
categories: [Sumo, Reference, 2025, January]
---

## Yokozuna
{% for wrestler in site.data.wrestlers.wrestlers %}{% if wrestler.rank == "Yokozuna" %}
- {{ wrestler.name }} ({{ wrestler.japanese_name }}) - [Videos](https://www.youtube.com/@sumo-video/search?query={{ wrestler.video_search }}) | [Profile]({{ wrestler.profile_url }}){% endif %}{% endfor %}

## Ozeki
{% for wrestler in site.data.wrestlers.wrestlers %}{% if wrestler.rank == "Ozeki" %}
- {{ wrestler.name }} ({{ wrestler.japanese_name }}) - [Videos](https://www.youtube.com/@sumo-video/search?query={{ wrestler.video_search }}) | [Profile]({{ wrestler.profile_url }}){% endif %}{% endfor %}

## Sekiwake
{% for wrestler in site.data.wrestlers.wrestlers %}{% if wrestler.rank == "Sekiwake" %}
- {{ wrestler.name }} ({{ wrestler.japanese_name }}) - [Videos](https://www.youtube.com/@sumo-video/search?query={{ wrestler.video_search }}) | [Profile]({{ wrestler.profile_url }}){% endif %}{% endfor %}

## Komusubi
{% for wrestler in site.data.wrestlers.wrestlers %}{% if wrestler.rank == "Komusubi" %}
- {{ wrestler.name }} ({{ wrestler.japanese_name }}) - [Videos](https://www.youtube.com/@sumo-video/search?query={{ wrestler.video_search }}) | [Profile]({{ wrestler.profile_url }}){% endif %}{% endfor %}

## Maegashira
{% for i in (1..17) %}{% for wrestler in site.data.wrestlers.wrestlers %}{% if wrestler.rank == "Maegashira" | append: i %}
- {{ wrestler.name }} ({{ wrestler.japanese_name }}) - [Videos](https://www.youtube.com/@sumo-video/search?query={{ wrestler.video_search }}) | [Profile]({{ wrestler.profile_url }}){% endif %}{% endfor %}{% endfor %}
