---
layout: default
title: Posts
---
<header class="intro">
    <h1>{{ page.title }}</h1>
</header>

<div class="case-studies-body">
    <ul class="listing">
        {% assign posts = site.posts | sort: 'application' %}
        {% for post-id in posts %}
        <li>
            <h2><a href="{{ post.application }}">{{ post.post-id }}</a></h2>
            {{ post.content }}
        </li>
        {% endfor %}
    </ul>
</div>