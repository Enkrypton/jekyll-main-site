---
layout: page
title: "Projects"
permalink: /projects/
---
 {% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url | absolute_url }}">
        {{ post.title }}
      </a>
    </h2>
	<p class="post-meta">
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%Y %B %d" }}</time>
	</p>
    {{ post.content }}
  </article>
{% endfor %}
