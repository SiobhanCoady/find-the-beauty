---
layout: default
---

<div class="gallery">
{% for post in site.posts limit: 9 %}
<div class="gallery-item">
<a href="{{ post.url | relative_url }}">
{% if post.featured_image %}
<img src="{{ post.featured_image | relative_url }}" alt="{{ post.title }}">
{% else %}
<div class="fallback-image"></div>
{% endif %}
<span>{{ post.title }}</span>
</a>
</div>
{% endfor %}
</div>
