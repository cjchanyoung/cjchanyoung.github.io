---
title: "Studies"
layout: single
permalink: /studies/
author_profile: true
---

#### 🏷️ Studies Tags
{% assign category_tags = site.categories.studies | map: 'tags' | join: ',' | split: ',' | uniq | sort %}
<div style="margin-bottom: 20px;">
  {% for tag in category_tags %}
    <a href="/tags/#{{ tag | slugify }}" class="btn btn--info btn--small">{{ tag }}</a>
  {% endfor %}
</div>

---

<div class="grid__wrapper">
  {% for post in site.categories.studies %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>