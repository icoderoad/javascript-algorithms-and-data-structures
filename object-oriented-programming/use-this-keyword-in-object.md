---
id: 605ada423daa59429d68d866
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 在对象中使用 this 关键字
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

在对象中使用 this 关键字

在上篇文件中我们了解了该如何给 site 对象设置一个方法属性。然后在 return 语句里，我们通过使用 “点号表示法” site.name来获取 name 的属性值：

welcomeMsg: function() {return "您好，菜鸟008。欢迎您访问" + site.name + "网站！";}

虽然这是访问对象属性的有效方法，但是这里有一个陷阱。如果变量名发生了改变，那么引用了原始名称的任何代码都需要更新。在一个简短的对象定义中这并不是问题，但是如果对象有很多对其属性的引用，那么发生错误的可能性就更大了。

在这个方法中，我们可以使用 this 关键字来避免这一问题：

let site = {
  name: "路条编程",
  domain: "www.icoderoad.com",
  url: "http://www.icoderoad.com",
  welcomeMsg: function() {return "您好，菜鸟008。欢迎您访问" + this.name + "网站！";}
};

console.log(  site.welcomeMsg() );
// => 您好，菜鸟008。欢迎您访问路条编程网站！


this 是一个很复杂的知识点，而上面那个例子也只是使用 this 的一种方法而已。在当前的上下文环境中，this 指向的就是与这个方法有关联的 site 对象。 

如果把对象的变量名改为 codeSite，那使用 this 就没有必要在代码中找到所有指向 site 的部分，这样可以使得代码更具有可读性和复用性。


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
