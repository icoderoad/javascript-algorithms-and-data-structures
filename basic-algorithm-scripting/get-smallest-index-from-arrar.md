---
id: 6054369200fc153fba31f8bb
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 返回将值插入数组后的最小索引
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

返回将值插入数组后的最小索引

今天我们介绍返回插入数组后的最小索引的方法。。在介绍具体方法之前，我们先介绍下数组的  concat()、sort() 和 indexOf() 方法。

concat() 方法用于合并两个或多个数组。此方法不会更改现有数组，而是返回一个新数组。

语法：

	var new_array = old_array.concat(value1[, value2[, ...[, valueN]]])

参数：

	valueN 可选，数组和/或值，将被合并到一个新的数组中。如果省略了所有 valueN 参数，则 concat 会返回调用此方法的现存数组的一个浅拷贝。详情请参阅下文描述。

返回值：
	新的 Array 实例。

sort() 方法用原地算法对数组的元素进行排序，并返回数组。默认排序顺序是在将元素转换为字符串，然后比较它们的UTF-16代码单元值序列时构建的

语法：

arr.sort([compareFunction])

参数：

compareFunction 可选，用来指定按某种顺序进行排列的函数。如果省略，元素按照转换为的字符串的各个字符的Unicode位点进行排序。

firstEl：第一个用于比较的元素。

secondEl：第二个用于比较的元素。

返回值：

排序后的数组。请注意，数组已原地排序，并且不进行复制。

indexOf() 方法返回在数组中可以找到一个给定元素的第一个索引，如果不存在，则返回-1。

语法：

arr.indexOf(searchElement[, fromIndex])

参数：

searchElement 要查找的元素

fromIndex 可选，开始查找的位置。如果该索引值大于或等于数组长度，意味着不会在数组里查找，返回-1。如果参数中提供的索引值是一个负值，则将其作为数组末尾的一个抵消，即-1表示从最后一个元素开始查找，-2表示从倒数第二个元素开始查找 ，以此类推。 

注意：如果参数中提供的索引值是一个负值，并不改变其查找顺序，查找顺序仍然是从前向后查询数组。如果抵消后的索引值仍小于0，则整个数组都将会被查询。其默认值为0.

返回值：

首个被找到的元素在数组中的索引位置; 若没有找到则返回 -1

实现步骤如下所示：

1、将 obj 插入 arr。

2、将 arr 进行升序排序。

3、返回 obj 的索引。


具体代码如下所示：

function getSmallestIndexFromArrary(arr, obj) {

	let newArray = arr.concat(obj)
	
	newArray.sort((a, b) => a - b)
	
	return newArray.indexOf(obj);
}

console.log( getSmallestIndexFromArrary([88, 66, 12], 50) );
// => 1 

console.log( getSmallestIndexFromArrary([2, 5, 13], 6) );
// => 2

console.log( getSmallestIndexFromArrary([], 1) );
// => 0

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
