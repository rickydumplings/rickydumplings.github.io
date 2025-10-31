---
# the default layout is 'page'
icon: fas fa-info-circle
order: 0
---

<!-- > Add Markdown syntax content to file `_tabs/about.md`{: .filepath } and it will show up on this page.
{: .prompt-tip } -->

Welcome! Here are some of my engineering projects.

<ul>
{% for post in site.categories.blog %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    — <small>{{ post.date | date: "%b %d, %Y" }}</small><br/>
    {{ post.excerpt }}
  </li>
{% endfor %}
</ul>
