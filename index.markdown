---
layout: default
title: Group Guided World Travel
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
<div class="action action-button inline-action-button">
<a href="{{ post.url | replace_first:'/','' }}">Learn More&nbsp;&gt;</a>
</div>
</div>
<div class="picture-book-page-image-author">
{{ post.hero-author }}
</div>
</div>
<div class="main-spacer">&nbsp;</div>
{% endif %}
        {% endfor %}
