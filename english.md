---
layout: layout
title: "English learning"
---

<div class="content">
  <h1>English Learning</h1>
  <ul class="listing">
    {% for post in site.posts %}
      {% unless post.draft %}
      <li>
        <span>{{ post.date | date: "%B %e, %Y" }}</span>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
      {% endunless %}
    {% endfor %}
  </ul>
</div>
