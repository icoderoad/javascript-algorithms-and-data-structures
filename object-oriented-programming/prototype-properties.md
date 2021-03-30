---
id: 6062b7370eeb64a83ef88b7b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 在对象中如何使用原型属性
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

在对象中如何使用原型属性

所有 Site 实例可能会有相同的 address 值，所以在每一个 Site 的实例中本质上都有一个重复的变量 address。

当只有两个实例时可能并不是什么问题，但想象一下如果有数百万个实例，这将会产生许多重复的变量。

这里有一个更好的方法可以解决上述问题，那就是使用 Site 的原型。原型是一个可以在所有 Site 实例之间共享的对象。

JavaScript 对象有一个指向一个原型对象的链。当试图访问一个对象的属性时，它不仅仅在该对象上搜寻，还会搜寻该对象的原型，以及该对象的原型的原型，依次层层向上搜索，直到找到一个名字匹配的属性或到达原型链的末尾。

遵循 ECMAScript 标准，someObject.[[Prototype]] 符号是用于指向 someObject 的原型。从 ECMAScript 6 开始，[[Prototype]] 可以通过 Object.getPrototypeOf() 和 Object.setPrototypeOf() 访问器来访问。这个等同于 JavaScript 的非标准但许多浏览器实现的属性 __proto__。

但它不应该与构造函数 func 的 prototype 属性相混淆。被构造函数创建的实例对象的 [[Prototype]] 指向 func 的 prototype 属性。Object.prototype 属性表示 Object 的原型对象。

以下是一个在 Site prototype 中添加 address 属性的示例：

Site.prototype.address = "北京市海淀区";

现在所有的 Site 实例都拥有了共同的 address 属性值，代码如下所示：

function Site(name) {
  this.name  = name;
}

Site.prototype.address = "北京市海淀区";

let icodeRoadSite = new Site("路条编程");

let qqSite = new Site("腾讯");


console.log(icodeRoadSite.address);  
// => 北京市海淀区

console.log(qqSite.address);  
// => 北京市海淀区

由于所有的实例都可以继承原型上的属性，所以可以把原型看作是创建对象的 "配方"。 请注意：icodeRoadSite 和 qqSite 的原型属于 Site 的构造函数，即 Site 的原型 Site.prototype。JavaScript 中几乎所有的对象都有一个原型属性，这个属性是属于它所在的构造函数。


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
