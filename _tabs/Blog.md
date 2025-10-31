---
layout: page
title: Blog
icon: fas fa-blog
order: 1
---



<!-- ---
layout: page
title: Blog
icon: fas fa-blog
order: 1
--- -->

Welcome! Here are some of my posts about topics and projects I've done that I found interesting.

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%b %d, %Y" }}</small>

{{ post.excerpt }}

---
{% endfor %}
