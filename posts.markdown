---
layout: default
---

{% for post in site.posts %}
<p>
<a href="{{ post.url | relative_url }}">
<strong>{{ post.title }}</strong>
</a>
{{ post.date | date: "%B %d, %Y" }}
</p>
{% endfor %}
