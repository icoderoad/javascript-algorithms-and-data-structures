---
id: 606425f659c4a6c138eb3695
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 迭代遍历对象所有属性
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

迭代遍历对象所有属性

到目前为止，您已经了解了对象的两种属性: 自身属性和原型属性。自身属性是直接在对象上定义的，而原型属性是定义在 prototype 上定义的。

function Site(name) {
  this.name = name;  // 自身属性
}

Site.prototype.address = "北京市海淀区"; // 原型属性

let icodeRoadSite = new Site("路条编程");

在介绍示例前，我们先介绍下对象的 hasOwnProperty 方法的用法. 

hasOwnProperty() 方法会返回一个布尔值，指示对象自身属性中是否具有指定的属性（也就是，是否有指定的键）。

语法:

obj.hasOwnProperty(prop)

参数:

prop 要检测的属性的 String 字符串形式表示的名称，或者 Symbol。

返回值:

用来判断某个对象是否含有指定的属性的布尔值 Boolean。

所有继承了 Object 的对象都会继承到 hasOwnProperty 方法。这个方法可以用来检测一个对象是否含有特定的自身属性；和 in 运算符不同，该方法会忽略掉那些从原型链上继承到的属性。

下面的示例将会说明如何将icodeRoadSite 的自身属性和原型属性分别添加到 ownProps 数组和 protoProps 数组里面：

let ownProps = [];
let protoProps = [];

for (let prop in icodeRoadSite) {
  if(icodeRoadSite.hasOwnProperty(prop)) {
    ownProps.push(prop);
  } else {
    protoProps.push(prop);
  }
}

console.log(ownProps); 
// => ["name"]

console.log(protoProps); 
// => ["address"]

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
