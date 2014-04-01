---
layout: page
title: "about"
---

The RedSnake is a meeting where Rubyists and Pythonistas get together to throw down some hard tech and inspire each other to level up. Ultimately we aim to accomplish the following:

1. To be the premier technical event for hardcore programmers in Philadelphia
1. To inspire and provide an environment of learning to those who are new to programming
1. To introduce Philadelphia's top companies to Philadelphia's top programmers
1. To raise national recognition for Philadelphia's tech community and attract top talent to the city


The format is 2 hours of alternating 10 minute lightning talks. It's intense, technical, and mind blowing.

<h3> Organizers </h3>

{% for post in site.categories.organizers %}
{% assign content = post.content %}
<div class="person">
  <div class="name">{{ post.name }}</div>
  {% if post.link_1 %}
  <div class="links">
  <a href="{{ post.link_1 }}" target="blank">{% if post.link_1_text %}{{post.link_1_text}}{% else %}{{ post.link_1 }}{% endif %}</a>
  {% if post.link_2 %}<a href="{{ post.link_2 }}" target="blank">{% if post.link_2_text %}{{post.link_2_text}}{% else %}{{ post.link_2}}{% endif %}</a>{% endif %}
  </div>
  {% endif %}
  <div class="pic"><img class="organizer" src="{{root_url}}/images/content/{{post.pic}}"/></div>
  <div>
  {{ post.bio }}
  </div>
</div>
<br class="spacer clear" />
{% endfor %}
