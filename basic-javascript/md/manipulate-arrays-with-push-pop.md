---
id: 5fc4b3e3af1c9298a2ef0e38
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:	使用 push()和pop()方法操作数组
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用 push()和pop()方法操作数组。

使用 push() 方法可向数组的末尾添加一个或多个元素，并返回数组新的长度。

语法如下所示：

array.push(element1,element2,....,elementn)

参数描述：

element1：必需，要添加到数组的第一个元素。

element2：可选，要添加到数组的第二个元素。

elementn：可选，可添加多个元素。

返回值：把指定的值添加到数组后的数组新长度。

var arrNames = new Array(3)
    arrNames[0] = "张三";
    arrNames[1] = "李四";
    arrNames[2] = "王五";

   console.log( arrNames.push("赵六")); // => 4
   console.log( arrNames); // => ["张三", "李四", "王五", "赵六"]

   控制台输出如下所示：
   4
   (4) ["张三", "李四", "王五", "赵六"]
   以上代码输出数组长度为 4， 表示新增元素后数组的长度，数组内容最后新增元素 “赵六”。

 使用 pop() 方法用来“抛出”一个数组末尾的值。可以把这个“抛出”的值赋给一个变量存储起来。换句话说就是 pop() 方法移除数组末尾的元素并返回这个元素。

 语法如下所示：

 array.pop()

返回值：array 的最后一个元素。

var cityArr = ["北京","杭州","上海"];
var city = cityArr.pop();
console.log(city); // => 上海
console.log(cityArr); // => (2) ["北京", "杭州"]


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
