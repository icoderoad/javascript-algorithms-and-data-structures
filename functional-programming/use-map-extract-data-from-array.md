---
id: 607fc0898dfa05ffd4a7f8ba
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 map 方法从数组中提取数据

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用 map 方法从数组中提取数据

目前为止，我们已经学会了使用纯函数来避免程序中的副作用。此外，我们还学习了函数的值仅取决于其输入参数等相关知识。

这仅仅是函数式编程的开始。后继我们还会学习很多实用的技巧解决实际工作中的问题。

能够将它们作为参数传递给其他函数，和从另一个函数返回一个函数是有意义的。函数在 JavaScript 中被视为第一类对象，它们可以像任何其他对象一样使用。它们可以保存在变量中，存储在对象中，也可以作为函数参数传递。

让我们从一些简单的数组函数开始，这些函数是数组对象原型上的方法。在本文章的示例练习中，我们来了解下数组的 map 方法（即Array.prototype.map()）。在介绍具体示例之前，我们先介绍下数组 map 方法的用法。

map() 方法创建一个新数组，其结果是该数组中的每个元素是调用一次提供的函数后的返回值。

语法：

var new_array = arr.map(function callback(currentValue[, index[, array]]) {
 // 返回新数组
}[, thisArg])

参数：

callback
	生成新数组元素的函数，使用三个参数：
	currentValue
		callback 数组中正在处理的当前元素。
	index可选
		callback 数组中正在处理的当前元素的索引。
	array可选
		map 方法调用的数组。
thisArg可选，执行 callback 函数时值被用作 this。


返回值：

一个由原数组每个元素执行回调函数的结果组成的新数组。


注意：map 方法是迭代数组中每一项的方式之一。在对每个元素应用回调函数后，它会创建一个新数组(不改变原来的数组)。

当调用回调函数时，传入了三个参数。第一个参数是当前正在处理的数组项，第二个参数是当前数组项的索引值，第三个参数是在其上调用 map 方法的数组。

看下在 sites 上使用 map 方法的例子，返回了一个新数组只包含了站点的名字。为了简化，例子里只使用了回调函数的第一个参数。

const sites = [
  { name: '腾讯', domain: "www.qq.com" },
  { name: '京东', domain: 'www.jd.com'},
  { name: '路条编程', domain: 'www.icoderoad.com' }
];

const names = sites.map(site => site.name);
console.log(names); 
// (3) ["腾讯", "京东", "路条编程"]

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
