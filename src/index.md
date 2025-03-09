---
title: Hello World!
layout: layout/base.njk
---
<html>

HI
<body><div>

hi
<p>hi</p>
{% for post in collections.blog | reverse | itemLimit(1) %}
<h1>{{ post.data.title }}</h1>
{{ post.content | safe }}
{% endfor %}
this should have worked tbh
</body>
</html>