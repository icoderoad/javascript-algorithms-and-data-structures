---
id: 5fc37589c37ea7e486f0bd5c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:	通过索引访问数组中的数据
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
通过索引访问数组中的数据。

上篇文章我们介绍了数组的创建及变量赋值，如何获取数组中的数据呢？在 JavaScript 语言中，我们可以使用索引 index 来访问数组中的数据。

数组索引与字符串索引一样使用中括号 []，通过字符串索引得到的是一个字符，而数组索引得到的是一个元素。数组索引与字符串索引一样是从 0 开始的，所以数组中第一个元素的索引编号是 0。
示例

var array = [30,60,90];
console.log( array[0] );  // => 30
var data = array[1];  
console.log( data ); // => 60

注意：数组名称和中括号之间不应有任何空格，如 array [0] 尽管 JavaScript 语言能够正确处理，但可能会让看你代码的其他程序员感到困惑。

与字符串的数据不可变不同，数组的数据是可变的，并且可以自由地改变。

修改数组数据示例如下所示：

var array = [30,60,90];
array[0] = 15; 
console.log(array);

控制台输出数据为 (3) [15, 60, 90]，表示数组里有 3 个数据，值分别为 15 60 90 。数组里第一个数据已经更新为 15。

通过索引不仅可以获取一维数组数据，还可以把多维数组看作一个数组中的数组。当使用中括号去访问数组的时候，第一个索引 [index] 访问的是第 N 个子数组，第二个 [index] 访问的是第 N 个子数组的第 N 个元素。

获取多维数组示例如下所示：

var arrs = [
  [1,2,3],
  [4,5,6],
  [7,8,9],
  [[10,11,12], 13, 14]
];
console.log( arrs[3] );  // => (3) [Array(3), 13, 14]
console.log( arrs[3][0] ) ; // => (3) [10, 11, 12]
console.log( arrs[3][0][1] ); // => 11

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
