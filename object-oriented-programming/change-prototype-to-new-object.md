---
id: 60667f3c3e93c83b44cc7a9d
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将对象原型更改为对象方式添加属性及方法
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

将对象原型更改为对象方式添加属性及方法

到目前为止，我们学到的相关知识，已经可以单独给对象的 prototype 添加属性，类似下面的代码：

function Site(name) {
  this.name = name;  // 自身属性
}

Site.prototype.address = "北京市海淀区";

如果通过这种方式给 Site 对象添加属性和方法，要添加的属性和方法很多时，这将在添加许多属性的时候变得单调乏味。

Site.prototype.about = function() {
  console.log("路条编程是一家介绍编程相关知识的网站");
}

Site.prototype.describe = function() {
  console.log("网站名称为 " + this.name);
}

let site = new Site("路条编程");

console.log( site.about() );
// => 路条编程是一家介绍编程相关知识的网站

console.log( site.describe() );
// => 网站名称为 路条编程

一种更有效的方法就是给对象的 prototype 设置为一个已经包含了属性的新对象。这样一来，所有属性都可以一次性添加进来，调整后的代码如下所示：

Site.prototype = {
  address: "北京市朝阳区", 
  about: function() {
    console.log("路条编程是一家介绍编程相关知识的社区");
  },
  describe: function() {
     console.log("我们网站的名称为 " + this.name);
  }
};

let site = new Site("路条编程");

console.log( site.about() );
// => 路条编程是一家介绍编程相关知识的社区

console.log( site.describe() );
// => 我们网站的名称为 路条编程

通过以上两种方法为对象添加相应的属性及方法，我们可以很明显看出，第二种通过新对象的方式结构更清晰。

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
