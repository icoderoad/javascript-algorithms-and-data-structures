---
id: 60584bb725cb676c8ffef923
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 在对象上创建方法
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

在对象上创建方法

对象可以有一个叫做方法的特殊属性。

方法其实是一个值为函数的属性，它可以为一个对象添加不同的行为。我们在上篇文章网站 site 对象的基础上，添加一个欢迎的方法，代码如下所示：

let site = {
  name: "路条编程",
  domain: "www.icoderoad.com",
  url: "http://www.icoderoad.com",
  welcomeMsg: function() {return "您好，菜鸟008。欢迎您访问" + site.name + "网站！";}
};

console.log(  site.welcomeMsg() );
// => 您好，菜鸟008。欢迎您访问路条编程网站！


这个例子给 site 对象添加了一个 welcomeMsg 方法，这个方法返回一个包含网站名字的欢迎信息。 

注意：这个方法在返回语句中使用 site.name 的方式来获取 name 的属性值。也可以使用另外一种方法来实现，我们会在后继文章中进行介绍。


</section>

## Instructions
<section id='instructions'>

</section>

## Tests
<section id='tests'>

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js

```

</div>



</section>

## Solution
<section id='solution'>


</section>
