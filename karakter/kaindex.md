---
layout: default
permalink: /karakter/
---

<div class="post row">
<h1>Tag: {{ page.karakter }}</h1>
<ul>
{% for post in site.karakter[page.karakter] %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date_to_string }})<br>
    {{ post.description }}
  </li>
{% endfor %}
</ul>
</div>