---
title: "Blog"
permalink: /blog/
layout: single
author_profile: true
---

#### 🏷️ Blog Tags
{% assign category_tags = site.categories.blog | map: 'tags' | join: ',' | split: ',' | uniq | sort %}
<div style="margin-bottom: 20px;">
  {% for tag in category_tags %}
    <a href="/tags/#{{ tag | slugify }}" class="btn btn--info btn--small">{{ tag }}</a>
  {% endfor %}
</div>

---

<div class="grid__wrapper">
  {% for post in site.categories.blog %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>