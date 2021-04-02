---
id: 6067aa890396cc9086a97c4b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 修改原链对构造函数的影响
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

修改原型对构造函数的影响

我们在上篇文章中介绍了手动给新对象重新设置原型对象相关的方法，此修改会产生一个重要的副作用，会删除对象的 constructor 属性！我们来看一下，我们以 Site 对象的实例 site 的为例，测试下 site 实例 constructor 属性输出到控制台相应结果，完整代码如下所示：

function Site(name) {
  this.name = name;  // 自身属性
}

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

console.log( site.constructor === Site ); 
// => false 

console.log( site.constructor === Object ); 
// =>true  /*所有的对象都继承自 Object.prototype */

console.log( site instanceof Site );
// =>true

为了解决对象的 constructor 属性被删除的问题，凡是手动给新对象重新设置过原型对象的，都别忘记在原型对象中定义一个 constructor 属性，修改后的代码如下所示：

Site.prototype = {
  constructor: Site,
  address: "北京市朝阳区", 
  about: function() {
    console.log("路条编程是一家介绍编程相关知识的社区");
  },
  describe: function() {
     console.log("我们网站的名称为 " + this.name);
  }
};

let newSite = new Site("路条编程");

console.log( newSite.constructor === Site ); 
// => true 

console.log( newSite.constructor === Object ); 
// => false  

console.log( newSite instanceof Site );
// => true

根据以上代码的输出结果可知，重新设置过原型对象的 constructor 属性后，constructor 返回了正确的对象类型。

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
