---
id: 605d8515b190a982a8e01c1e
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用构造函数创建对象
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用构造函数创建对象

在上篇文章中，我们用所学到的知识创建了一个 Site 构造函数：

function Site() {
  this.name = "路条编程";
  this.domain = "www.icoderoad.com";
  this.address = "北京市海淀区";
   // 构造器内的 "this" 一直指向创建的对象
}

let codeRoadSite = new Site();

注意：通过构造函数创建对象的时候要使用 new 操作符。因为只有这样，JavaScript 才知道要给 Site 这个构造函数创建一个新的实例：codeRoadSite。如果不使用 new 操作符来新建对象，那么构造函数里面的 this 就无法指向新创建的这个对象实例，从而产生不可预见的错误。 现在 codeRoadSite 这个实例就继承了  Site 这个构造函数的所有属性，如下：

console.log(codeRoadSite.name); 
// => 路条编程

console.log(codeRoadSite.domain); 
// => www.icoderoad.com

console.log(codeRoadSite.address); 
// => 北京市海淀区


由构造函数创建的实例也和其他对象一样，它的属性可以被访问和修改：

codeRoadSite.name = '路条公众号';
console.log(codeRoadSite.name); 
// => 路条公众号


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
