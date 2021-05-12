---
id: 60961647ba50c85eb90c93fe
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 返回这两个数组的对称差
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

返回这两个数组的对称差

本次练习我们需要写一个函数，比较两个数组，返回一个新的数组。这个新数组需要包含传入的两个数组所有元素中，仅在其中一个数组里出现的元素。如果某个元素同时出现在两个数组中，则不应包含在返回的数组里。换言之，我们需要返回这两个数组的对称差。

注意：返回数组中的元素可任意排序。


在介绍完整代码之前，我们先介绍下数组 indexOf() 方法的具体用法：

indexOf()方法返回在数组中可以找到一个给定元素的第一个索引，如果不存在，则返回-1。

语法：
arr.indexOf(searchElement[, fromIndex])

参数：
	searchElement
		要查找的元素

	fromIndex 可选
		开始查找的位置。如果该索引值大于或等于数组长度，意味着不会在数组里查找，返回-1。如果参数中提供的索引值是一个负值，则将其作为数组末尾的一个抵消，即-1表示从最后一个元素开始查找，-2表示从倒数第二个元素开始查找 ，以此类推。 

注意：如果参数中提供的索引值是一个负值，并不改变其查找顺序，查找顺序仍然是从前向后查询数组。如果抵消后的索引值仍小于0，则整个数组都将会被查询。其默认值为0.

返回值：
首个被找到的元素在数组中的索引位置; 若没有找到则返回 -1


我们定义一个方法 diffArray ， 该方法包含两个参数，分别为 arr1 和 arr2 ，该方法返回这两个数组的对称差的新数组。具体代码如下所示：

function  diffTwoArray( arr1, arr2 ){
	var newArr = [];

    for (var i = 0; i < arr1.length; i++) {
      if (arr2.indexOf(arr1[i]) === -1) {
        newArr.push(arr1[i]);
      }
    }

    for (var i = 0; i < arr2.length; i++) {
      if (arr1.indexOf(arr2[i]) === -1) {
        newArr.push(arr2[i]);
      }
    }

  return newArr;
}

var newArr = diffTwoArray([11, 31, 52, 71], [71, 2, 52, 4, 31]);
console.log(newArr);
// => (3) [11, 2, 4]

newArr = diffTwoArray(['路条编程', '阿里巴巴', '拼多多', '亚马逊'], ['京东', '美团', '拼多多', '头条', '亚马逊']);
console.log(newArr);
// => (5) ["路条编程", "阿里巴巴", "京东", "美团", "头条"]

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
