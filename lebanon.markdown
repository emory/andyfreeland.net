---
layout: default
title: Lebanon
---

<h1 id="archive">Lebanon</h1>

I'm studying Arabic in Lebanon from 2 September 2010 through 12 December 2010. It'll be pretty awesome.

Here you can see everything I've written about it. With pictures!

<ol class="archive">
    {% for post in site.categories.lebanon %}
    <li>
        <span class="date">{{ post.date | date_to_string }}</span>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
</ol>
