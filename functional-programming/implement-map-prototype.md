---
id: 607fc0898dfa05ffd4a7f8ba
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 在原型上实现 map 方法

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

在原型上实现 map 方法

我们之前用 map 方法（即 Array.prototype.map() ）返回一个与调用它的数组长度相同的数组。只要它的回调函数不改变原始数组，它就不会改变原始数组。

换句话说，map 是一个纯函数，它的输出仅取决于输入的数组和作为参数传入的回调函数。

为了加深对 map 方法的理解，现在我们来用 for 或 Array.prototype.forEach() 自己实现一下这个方法。

注意：纯函数可以改变其作用域内定义的局部变量，但我们最好不要这样做。

写一个和 Array.prototype.map() 一样的 Array.prototype.myMap()。可以用 for 循环或者 forEach 方法。

在介绍实例之前，先介绍下 Array 数组 forEach() 方法。

forEach() 方法对数组的每个元素执行一次给定的函数。

语法：

arr.forEach(callback(currentValue [, index [, array]])[, thisArg])

参数：

callback 为数组中每个元素执行的函数，该函数接收一至三个参数：

	currentValue
		数组中正在处理的当前元素。

	index 可选
		数组中正在处理的当前元素的索引。

	array 可选
		forEach() 方法正在操作的数组。

thisArg 可选，可选参数。当执行回调函数 callback 时，用作 this 的值。

返回值：
	undefined。

var numArr = [7, 13, 31, 53];

Array.prototype.eachMap = function(callback) {

  var newArray = [];

  this.forEach(num => newArray.push(callback(num)));
 
  return newArray;
};

var tmpArr = numArr.eachMap(function(num) {
  return num * 2;
});

console.log( tmpArr );
// => (4) [14, 26, 62, 106]

以上代码实现一个自定义的 eachMap 方法，实现对数组每个元素变为原值的 2 倍，最终将处理后的元素存放在数组 tmpArr 中，然后将数组在控制台输出。

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
