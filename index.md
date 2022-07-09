---
layout: portfolio
---

# Portfolio

#### Take a look at what I am working on right now:

<ul>
  {% for project in site.projects %}
    {% if project.current == true %}
      <li class="projects_li">
        <a href="{{ project.url }}">
          {{ project.title }}
        </a> - {{ project.technology }}<br>
        <span class="projects_desc">{{ project.description }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>

#### Take a look at some of the projects I have worked on in the past:

<ul>
  {% for project in site.projects %}
    {% if project.current == false %}
      <li class="projects_li">
        <a href="{{ project.url }}">
          {{ project.title }}
        </a> - {{ project.technology }}<br>
        <span class="projects_desc">{{ project.description }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>

#### Other interests:

<ul>
      <li class="projects_li">
        <a target="_blank" href="https://www.artstation.com/icouldbreathe">
          3D Modelling: ArchStation Portfolio
        </a> - Blender<br>
        <span class="projects_desc">On the path of learning 3D modelling. ArchStation Portfolio.</span>
      </li>
</ul>


{% if site.posts_enabled %}

---

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