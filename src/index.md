---
title: Hello World!
layout: layout/base.njk
---

<p>
  Check out your cool new static site built with
  <a href="https://11ty.dev">11ty</a> on
  <a href="https://neocities.org/">Neocities</a>.
</p>

<p>omg lol</p>

<ul>
  <li>Creating your own space on the web</li>
  <li>Expressing yourself</li>
  <li>Displaying all the gifs you've collected</li>
</ul>

<h2>Why do you want a homepage?</h2>
<p>The web was made for personal homepages, make this one yours</p>

{% set postslist = collections.posts | head(-1) %}

{% for post in postslist | head(-1) %}
  <h1>{{ post.data.title }}</h1>
  {{ post.templateContent | safe }}
{% endfor %}
