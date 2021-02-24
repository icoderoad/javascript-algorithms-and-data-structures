---
id: 6035e440de1369c351fc854c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 indexOf() 检查元素是否存在
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 indexOf() 检查元素是否存在

由于数组可以在任意时间被修改或者说被改变，我们不能保证某个数据在一个给定数组中的位置，甚至不能保证该元素还存在于该数组中。幸运的是，JavaScript 语言 给我们提供了另一个内置方法 indexOf()。这个方法让我们可以便捷地检查某个元素是否存在于一个数组中。

indexOf() 方法返回在数组中可以找到一个给定元素的第一个索引，如果不存在，则返回-1。

语法：arr.indexOf(searchElement[, fromIndex])

参数：

searchElement 要查找的元素
fromIndex 可选

开始查找的位置。如果该索引值大于或等于数组长度，意味着不会在数组里查找，返回 -1。如果参数中提供的索引值是一个负值，则将其作为数组末尾的一个抵消，即-1 表示从最后一个元素开始查找，-2 表示从倒数第二个元素开始查找 ，以此类推。 

注意：如果参数中提供的索引值是一个负值，并不改变其查找顺序，查找顺序仍然是从前向后查询数组。如果抵消后的索引值仍小于0，则整个数组都将会被查询。其默认值为 0.

返回值：首个被找到的元素在数组中的索引位置; 若没有找到则返回 -1

下面我们做个简单的示例：

let welcomeMsgs = ["您好", "菜鸟001", "欢迎", "访问", "路条编程"];

let result = welcomeMsgs.indexOf('icoderoad'); 
console.log( result );
// => 返回 -1

result= welcomeMsgs.indexOf('菜鸟001'); 
console.log( result );
// => 返回 1

result = welcomeMsgs.indexOf('路条编程'); // 
console.log( result );
// => 返回 4，即第一个出现的 '路条编程' 元素在数组中的索引为 4

indexOf() 方法在快速检查一个数组中是否存在某个元素时非常有用。

下面我们来做个完整的练习，定义一个 quickCheck 函数，它接受一个数组和一个元素作为输入参数。利用 indexOf()方法，使得当输入的数组中含有输入的元素时，函数返回 true；不含有输入的元素时，函数返回 false。

function quickCheck(arr, elem) {

  let result = arr.indexOf( elem ) >= 0 ? true : false;
  return result;

}

let checkArr = ["您好", "菜鸟001", "欢迎", "访问", "路条编程"];
let exist = quickCheck(checkArr , "菜鸟008");
console.log( exist );
// => false

exist = quickCheck(checkArr , "路条编程");
console.log( exist );
// => true


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
