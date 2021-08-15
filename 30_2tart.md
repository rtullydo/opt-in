---
layout: page
title: "2TART"
permalink: "index.html"
---



![2tart](assets/images/2tart-crop.png)

Welcome to **The Online Operator Theory and Related Topics** webpage. This project intends to provide accessible colloqium-level operator theory talks on a monthly basis (currently the first Tuesday of each month at 11AM Eastern (US)), with occasional additional talks. This project is co-ordinated by J. E. Pascoe. If you want to be added to the mailing list, please email the organizers.

  {% for post in site.posts %}
  <article>
    <h2>
      <a href="https://operatortheory.org/{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}