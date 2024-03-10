---
title: My Second Eleventy Site
layout: base.njk
---

## Interesting content
this is where the intereseting content lives
but this time it's using a markdown file

## Second paragraph
this is some more really intesting content
but this time it's also using a markdown file

## Third paragraph
This is to check the automatic re-deploy

{% for blog in collections.blogs  %}
<div class="blog-item">
    <a href="{{blog.url}}">{{ blog.data.title}}</a>
    <p>{{ blog.content }}</p>
</div>
<p>&nbsp;<p>
{%endfor%}
