---
layout: default
---

# Portfolio

Take a look at some projects I have worked on.

<ul>
  {% for project in site.projects %}
    <li>
      <a href="{{ project.url }}">
        {{ project.title }}
      </a> - {{ project.technology }}
      <p>{{ project.description }}</p>
    </li>
  {% endfor %}
</ul>

{% if site.posts_enabled %}
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
  {% endfor %}
</ul>
{% endif %}