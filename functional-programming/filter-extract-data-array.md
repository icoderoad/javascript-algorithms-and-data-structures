---
id: 60826a79a46e25724b800c62
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组对象 filter 方法从数组中提取数据
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组对象 filter 方法从数组中提取数据

在日常工作中另一个比较有用的数组方法是 filter()（即Array.prototype.filter()）。filter() 方法创建一个新数组, 其包含通过所提供函数实现的测试的所有元素。 


和 map() 方法一样，filter() 方法不会改变原始数组，它接收一个回调函数，将回调内的逻辑应用于数组的每个元素。新数组包含根据回调函数内条件返回 true 的元素。

回调函数接收三个参数。第一个参数是当前正在被处理的元素，第二个参数是元素的索引，第三个参数是在其上调用 filter 方法的数组。 具体用法如下所示：

语法：

var newArray = arr.filter(callback(element[, index[, array]])[, thisArg])

参数：

callback
	用来测试数组的每个元素的函数。返回 true 表示该元素通过测试，保留该元素，false 则不保留。它接受以下三个参数：

	element
		数组中当前正在处理的元素。

	index 可选
		正在处理的元素在数组中的索引。

	array 可选
		调用了 filter 的数组本身。

thisArg 可选，执行 callback 时，用于 this 的值。

返回值：

一个新的、由通过测试的元素组成的数组，如果没有任何数组元素通过测试，则返回空数组。


看下在 site 上使用 filter 方法的例子，返回了一个新数组包含了 30 岁以下的用户。为了简化，例子里只使用了回调函数的第一个参数。

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

const siteArr = sites.filter(site => site.userNum < 200);
console.log(siteArr); 
// => 0: {name: "路条编程", domain: "www.icoderoad.com", userNum: 150}

以上代码对站点数组进行过滤， 过滤出员工数小于200人的网站，将过滤结果赋值给变量 siteArr，然后在控制台将过滤结果输出。

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
