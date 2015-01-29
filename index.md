---
layout: page
title: Welcome on board, soldier
tagline: This is viking speaking
---
{% include JB/setup %}

###I am a frond-end developer, I can write HTML+CSS+Javascript code with maintainability readability, and modularity.
    
## Resumes
<ul class="listing">
<li>
  <span>Last updated 2015/01/28</span> <a href="http://vikingmute.github.com/resume.html">中文版</a>
</li>
<li>
  <span>Last updated 2013/08/01</span> <a href="http://vikingmute.github.com/resume_en.html">English version</a>
</li>
</ul>

## Posts
<ul class="listing">
{% for post in site.posts %}
<li>
  <span>{{ post.date | date: "%B %e, %Y" }}</span> <a href="{{ post.url }}">{{ post.title }}</a>
</li>
{% endfor %}
</ul>








