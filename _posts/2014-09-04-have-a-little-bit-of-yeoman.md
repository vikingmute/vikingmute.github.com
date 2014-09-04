---
layout: post
title: "Have a little bit of Yeoman"
description: ""
category: 
tags: ['Javascript']
---
{% include JB/setup %}

## Have a little bit of Yeoman

Using yeoman to build your project is simple and elegant, check it out. 

This is also a memo for me. You can check the offical website for more infomation.

[Yeoman website] (http://yeoman.io/learning/)

#### Install da tools
{% highlight bash %}
# install the yo
$ npm install -g yeoman 
# if npm version under 1.2.10
$ npm install -g grunt-cli bower
{% endhighlight %}

#### Install a generator
{% highlight bash %}
# install webapp generator
$ npm install -g generator-webapp
{% endhighlight %}

#### Create your app
{% highlight bash %}
$ mkdir project
$ cd project
$ yo webapp
{% endhighlight %}

#### Install packages
{% highlight bash %}
# install and save package name into bower.json
$ bower install backbone --save
# check your installed packages
$ bower list
# automatic write your deps into index.html using grunt
$ grunt bowerInstal
# open your index.html and check it out
$ vim index.html
{% endhighlight %}

#### Liveload code changes
{% highlight bash %}
# to be continued ...
{% endhighlight %}

#### Build your code
{% highlight bash %}
#check out your current grunt jobs 
$ grunt --help
# start a server
$ grunt serve
# build your code from app to dist
$ grunt build
{% endhighlight %}

