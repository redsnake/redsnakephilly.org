---
layout: page
title: "speakers"
---

Our speaker list is almost complete! In addition to all these below, we've got talks about Salt Stack, what's new in Python and Ruby, Blinker, and "putting a REPL on it."

{% assign index = true %}

{% for post in site.categories.speakers %}
{% assign content = post.content %}
<div class="speaker">
  <div class="title">{{ post.title }}</div>
  {% if post.author_image %}
  <div class="pic" ><img alt="{{ post.author }}" src="{{root_url}}/images/speakers/{{ post.author_image }}"/></div>
  {% endif %}
  <div class="author">{{ post.author }}</div>
  <div class="abstract">{{ post.abstract }}</div>
  <div class="bio">{{ post.bio }}</div>
</div>
  <br class="spacer clear" />
{% endfor %}
