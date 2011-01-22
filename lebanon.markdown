---
layout: default
title: Lebanon
---

<h1 id="archive">Lebanon</h1>

I spent fall term 2010 in Beirut, Lebanon studying Arabic at [Lebanese American University](http://www.lau.edu.lb/centers-institutes/sinarc/). It was wonderful. Those 15 weeks were probably the best experience of my life.

Sadly, there's still a few things I haven't written about, but I might add those someday.

Here you can see everything I've written about it. With pictures!

<ol class="archive">
    {% for post in site.categories.lebanon %}
    <li>
        <span class="date">{{ post.date | date_to_string }}</span>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
</ol>
