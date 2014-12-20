---
layout: page
title: "sponsors"
---

Want to sponsor this awesome event? Email <a href="mailto:info@redsnakephilly.org"> info@redsnakephilly.org </a> !

{% assign index = true %}

{% for post in site.categories.sponsors %}
{% assign content = post.content %}
<h2 style="margin-bottom:10px;">{{ post.sponsored }}</h2>
<div class="post">
  <div class="pic" ><a href="{{post.sponsor_url}}"><img alt="{{ post.name }}" src="{{root_url}}/images/sponsors/{{ post.logo }}"/></a></div>
  <br/>
  <p class="text">{{ post.blurb }}</p>
</div>
<br class="spacer clear" />
{% endfor %}
