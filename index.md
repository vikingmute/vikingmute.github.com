---
layout: page
title: Welcome on board, soldier
tagline: This is viking speaking
---
{% include JB/setup %}


## 牛逼的markdown 牛逼的github 牛逼的jekyll

用markdown的感觉真好 每个程序员都应该有一个github的静态博客啊~

原来的博客还是会写 毕竟东西太多了 导过来也比较麻烦 这里用来写一些翻译的作品和原创的小说 还会把简历 项目经验 什么的放过来  
    
## Sample Posts

This blog contains sample posts which help stage pages and blog data.
When you don't need the samples anymore just delete the `_posts/core-samples` folder.

    $ rm -rf _posts/core-samples

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



