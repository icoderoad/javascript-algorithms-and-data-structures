---
id: 608b647751e01039f2a3adfc
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组 sort 方法按字母顺序给数组排序
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组 sort 方法按字母顺序给数组排序

今天给大家介绍数组排序相关的知识，在介绍具体示例之前，我们先熟悉下数组 sort() 方法的相关知识。

sort() 方法用原地算法对数组的元素进行排序，并返回数组。默认排序顺序是在将元素转换为字符串，然后比较它们的UTF-16代码单元值序列时构建的

语法：
arr.sort([compareFunction])

参数：

compareFunction 可选
	用来指定按某种顺序进行排列的函数。如果省略，元素按照转换为的字符串的各个字符的Unicode位点进行排序。
	firstEl
		第一个用于比较的元素。
	secondEl
		第二个用于比较的元素。

返回值：
排序后的数组。请注意，数组已原地排序，并且不进行复制。

描述：
如果没有指明 compareFunction ，那么元素会按照转换为的字符串的诸个字符的 Unicode 位点进行排序。例如 "baidu" 会被排列到 "icoderoad" 之前。当数字按由小到大排序时，9 出现在 80 之前，但因为（没有指明 compareFunction ），比较的数字会先被转换为字符串，所以在 Unicode 顺序上 "80" 要比 "9" 要靠前。

如果指明了 compareFunction ，那么数组会按照调用该函数的返回值排序。即 a 和 b 是两个将要被比较的元素：

如果 compareFunction(a, b) 小于 0 ，那么 a 会被排列到 b 之前；
如果 compareFunction(a, b) 等于 0 ， a 和 b 的相对位置不变。备注： ECMAScript 标准并不保证这一行为，而且也不是所有浏览器都会遵守（例如 Mozilla 在 2003 年之前的版本）；
如果 compareFunction(a, b) 大于 0 ， b 会被排列到 a 之前。
compareFunction(a, b) 必须总是对相同的输入返回相同的比较结果，否则排序的结果将是不确定的。

现在我们练习一个完整的示例，具体代码如下所示：

举个例子：

function ascOrderArr(arr) {
  return arr.sort(function(a, b) {
    return a - b;
  });
}

var newArr = ascOrderArr([11, 51, 23, 35, 42]);
console.log( newArr );
// => (5) [11, 23, 35, 42, 51]


function reverseAlpha(arr) {
  return arr.sort(function(a, b) {
    return a === b ? 0 : a < b ? 1 : -1;
  });
}

console.log( reverseAlpha(['baidu.com', 'tmall.com', 'cctv.com', 'icoderoad.com', 'qq.com']));
// => (5) ["tmall.com", "qq.com", "icoderoad.com", "cctv.com", "baidu.com"]

JavaScript 的默认排序方法是 Unicode 值顺序排序，有时可能会得到意想不到的结果。所以，建议传入一个回调函数指定数组项目的排序方式，这个回调函数通常叫做 compareFunction 排列方法，它根据 compareFunction 排列方法的返回值决定数组元素的排序方式： 如果两个元素 a 和 b，compareFunction(a,b) 返回一个比 0 小的值，那么 a 会在 b 的前面。 如果两个元素 a 和 b，compareFunction(a,b) 返回一个比 0 大的值，那么 b 会在 a 的前面。 如果两个元素 a 和 b，compareFunction(a,b) 返回等于 0 的值，那么 a 和 b 的位置保持不变。

我们再对上面 reverseAlpha 方法进行调整，调整为按域名首字母的字母顺序排列进行排列，调整后的代码如下所示：

function alphaSortSite( arr ){
	return arr.sort(function(a, b) {
    return a === b ? 0 : a < b ? -1 : 1;
  });
}

console.log( alphaSortSite(['baidu.com', 'tmall.com', 'cctv.com', 'icoderoad.com', 'qq.com']));
// => (5) ["baidu.com", "cctv.com", "icoderoad.com", "qq.com", "tmall.com"]

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
