---
id: 605ec475401d938a63e35759
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 instanceof 验证对象构造函数
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 instanceof 验证对象构造函数

凡是通过构造函数创建出的新对象，都叫做这个构造函数的实例。JavaScript 提供了一种很简便的方法来验证对象的构造函数，那就是通过 instanceof 运算符用于检测构造函数的 prototype 属性是否出现在某个实例对象的原型链上。 

语法：

object instanceof constructor

参数：

object 某个实例对象
constructor 某个构造函数


instanceof 操作符允许将对象与构造函数之间进行比较，根据对象是否由这个构造函数创建的返回 true 或者 false。以下是一个示例：

let Site = function (name, domain) {
  this.name = name;
  this.domain = domain;
  this.address = "北京市海淀区";
}

let qqSite = new Site("腾讯", "www.qq.com");

 console.log( qqSite instanceof Site ); 
 // => true

如果一个对象不是使用构造函数创建的，那么 instanceof 将会验证这个对象不是构造函数的实例：

let icoderoad = {
  name: "路条编程",
  domain: "www.icoderoad.com",
  address: "北京市海淀区";
};

console.log( icoderoad instanceof Site ) ; 
// => false

需要注意的是，如果表达式 obj instanceof Site 返回 true，则并不意味着该表达式会永远返回 true，因为 Site.prototype 

属性的值有可能会改变，改变之后的值很有可能不存在于 obj 的原型链上，这时原表达式的值就会成为 false。另外一种情况下，原表达式的值也会改变，就是改变对象 obj 

的原型链的情况，虽然在目前的 ES 规范中，我们只能读取对象的原型而不能改变它，但借助于非标准的 __proto__ 伪属性，是可以实现的。比如执行 obj.__proto__ = {} 

之后，obj instanceof Site 就会返回 false 了。

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
