---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

# Welcome to My Jekyll Site

This is the home page of my Jekyll-powered website. Here, you can provide a brief introduction, share some information about yourself or your project, and showcase recent posts.

## Latest Posts

{% for post in site.posts %}
<h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
<p>{{ post.date | date: "%b %-d, %Y" }}</p>

{% if post.featured_image %}
<img src="{{ post.featured_image | relative_url }}" alt="{{ post.title }}">
{% endif %}
{% endfor %}
