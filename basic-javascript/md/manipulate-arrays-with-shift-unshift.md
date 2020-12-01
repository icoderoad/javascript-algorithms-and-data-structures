---
id: 5fc6167f3b237c4505e80c3f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:	使用 shift()和 unshift()方法操作数组
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用 shift()和 unshift()方法操作数组。

pop() 方法用来移出数组中最后一个元素。如果想要移出第一个元素要怎么办呢？

这就是 shift() 方法的用武之地。它的工作原理就像 pop()方法 ，但它移除的是第一个元素，而不是最后一个。

shift() 方法从数组中删除第一个元素，并返回该元素的值。此方法更改数组的长度。

语法如下所示：

arr.shift()

返回值：从数组中删除的元素; 如果数组为空则返回 undefined 。

示例如下所示：

var arrNames = new Array(3)
    arrNames[0] = "张三";
    arrNames[1] = "李四";
    arrNames[2] = "王五";

   console.log( arrNames); // => ["张三", "李四", "王五"]
   arrNames.shift();
   console.log( arrNames); // => ["李四", "王五"]

不仅可以 shift()方法移出数组中的第一个元素，也可以 unshift()方法插入一个元素到数组的头部。

.unshift() 方法用起来就像 push() 方法一样, 但不是在数组的末尾添加元素，而是在数组的头部添加元素。

 语法如下所示：

 arr.unshift(element1, ..., elementN)

 参数列表
    element1 要添加到数组开头的第一个元素
    elementN 要添加到数组开头的第 N 个元素

返回值：当一个对象调用该方法时，返回其 length 属性值。

示例如下所示：

var cityArr = ["北京","杭州","上海"];
console.log(cityArr); // => (3) ["北京", "杭州", "上海"]
cityArr.unshift("深圳");
console.log(cityArr); // => (4) ["深圳", "北京", "杭州", "上海"]


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
