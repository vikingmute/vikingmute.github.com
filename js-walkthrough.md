---
layout: page
title: "Js Walkthrough"
description: "my personal javascript walkthrough"
---
{% include JB/setup %}

#Javascript知识结构

##基础

* 基本类型 String Array Boolean Number Object Function
* 每个类型的内置函数（ECMA5新加的一些array的函数之类）
* Date类型 Regex类型的一些方法和用法（两日期之间相隔天数基本正则等等）
* 流程控制（if else for while)之类
* 任务 做一个类似underscore的数组小工具类 写两三方法即可

Api like this
_v.each()  _v.filter()  _v.some()....

##DOM+BOM

* Dom基本方法和操作 （查找 添加属性 删除属性 父元素 子元素 插入新元素 在特定位置插入新元素 删除元素 样式表操作）
* 基于浏览器的一些方法（setTimeout setInterval window.open() window.location navigator之类）
* document forms的一些操作 对radio  dropdownlist checkbox一系列的操作
* cookie是什么 怎么操作
* 任务 完成一个类似jquery的小选择器库（可以使用querySelectorAll）

大体上的api：
V('id')  V('id').remove() V('id').parent()  V('id').child()  V('id').addClass() V('id').attribute()

##Events

* Dom一级事件 和 Dom二级事件分别是什么 ie下dom二级事件的兼容性问题
* 事件中的事件对象 都有什么重要属性和方法  在不同浏览器下 有什么区别
* 事件代理是怎么回事？ 怎么样实现的呢？
* 事件冒泡和事件捕获是什么东西（什么元素 事件 不会冒泡？）
* 自定义事件 你怎么理解？
* 写一个小事件库 支持自定义事件 事件代理等方法(可以考虑考虑兼容性 不考虑也无所谓)

大体上的api
V.events.add() V.events.remove()  V.events.delegate() V.events.trigger() V.events.custom()

##Ajax

* 什么是ajax  什么是xmlHttpRequest
* 怎么运作的 写点代码来实现一个简单的xhr(考虑点兼容性)
* 了解HTTP （可以独立出ajax章节 作为必须考的其他的话题深入 具体流程 过程 再往下 三层模型之类 越详细越好）- 详见下面的高级话题
* 跨域问题 什么意思 子域名跨域有问题吗？
* 跨域问题解决 get请求 jsonp  post请求（xhr二级定义+老浏览器原始解决方法）
* json的概念和示例
* ajax的promise格式是指什么 
* 写一个简单库 来实现基本的ajax功能(基本的和promise的都可以～)
V.ajax({url:'a',method:'GET',dataType:'json',data:{'name':viking}},function(data){
       console.log(data)
})

##高级话题
* js的代码复用模式 （传统继承和现代继承）详见javascript模式一书第六章
* 你所理解的闭包（closure）是什么 有什么应用场景 解决些什么问题
* 好好读下javascript秘密花园里面的内容 http://bonsaiden.github.io/JavaScript-Garden/zh/
* js的一些常见设计模式 javascript模式一书 第七章
* YUI2的基本思路（多层命名空间）+ YUI3的基本思路（沙箱+动态加载模块）上面书的第五章 可以看看
* module模式 commonJS AMD CMD区别于联系 一些Module开发的库的了解 sea.js requeire.js的问题
* HTTP的基本原理 建议看一下 http://net.tutsplus.com/tutorials/tools-and-tips/http-the-protocol-every-web-developer-must-know-part-1/ 还有一个PART 2也必须看
* 同上一条 了解重要的一些http request header和repsonse header代表的意义 了解cache（缓存）的工作原理 （一些关于cache的http标准头的含义 Cache-control Expires) 
* 了解Browser的工作原理 了解repaint 和 reflow的区别 参考耗子的：http://coolshell.cn/articles/9666.html

待续...
