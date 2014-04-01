---
layout: page
title: "sponsors"
---

Want to sponsor this awesome event? Email <a href="mailto:info@redsnakephilly.org"> info@redsnakephilly.org </a> !

{% assign index = true %}

{% for post in site.categories.sponsors %}
{% assign content = post.content %}
<div class="speaker">
  <a href="{{ post.url }}>
  <img class="pic" style="float:left; width:250px; margin-right:25px;" alt="{{ post.name }}" src="{{root_url}}/images/sponsors/{{ post.logo }}"/>
  </a>
  <p class="text" style="margin-top:50px;">{{ post.blurb }}</p>
</div>
<br class="spacer clear" />
{% endfor %}
