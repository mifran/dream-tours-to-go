---
layout: default
title: Group Escorted Cruises
this-button: Tours
---
        {% for post in site.posts reversed %}
{% if post.type == "tour" %}
<div class="page">
<div class="picture-book-page-image">
<img src="{{ post.hero-image }}" alt="{{ post.hero-alt }}"/>
</div>
<div class="picture-book-page-text">
<header>
{{ post.hero-text }}
</header>
<div class="action action-button">
<a href="{{ post.url | replace_first:'/','' }}">Learn More&nbsp;&gt;</a>
</div>
</div>
<div class="picture-book-page-image-author">
{{ post.hero-author }}
</div>
</div>
{% endif %}
        {% endfor %}
