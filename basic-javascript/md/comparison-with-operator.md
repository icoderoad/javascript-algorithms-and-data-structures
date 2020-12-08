---
id: 5fcf10139f5525713e222b01
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 关系运算符之比较运算
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
关系运算符之比较运算。

在JavaScript 语言中，用于进行比较的关系运算符包含：小于(<)、大于(>)、小于等于(<=)、大于等于(>=)、相等(==)、不等(!=)、全等(恒等)(===)、不全等(不恒等)(!==)。前面文章中我们已经介绍了相等(==)、不等(!=)、全等(恒等)(===)、不全等(不恒等)(!==)四种关系运算。现在我们介绍小于(<)、大于(>)、小于等于(<=)、大于等于(>=)四种比较运算。

大于运算符 (>)

使用大于运算符（>）来比较两个数字。如果大于运算符左边的数字大于右边的数字，将会返回 true，否则，它返回 false。

语法示例如下所示：

x > y

与相等运算符一样，大于运算符在比较的时候，会转换值的数据类型。

例如

console.log( 5   >  3   ); // => true
console.log( 7   > '3'  ); // => true
console.log( 2   >  3   ); // => false
console.log( '1' >  9   ); // => false

大于等于运算符 (>=)

使用大于等于运算符（>=）来比较两个数字的大小。如果大于等于运算符左边的数字比右边的数字大或者相等，它会返回 true，否则，它会返回 false。

语法示例如下所示：

x >= y

与相等运算符相似，大于等于运算符在比较的时候会转换值的数据类型。

例如

console.log( 6   >=  6   ); // => true
console.log( 7   >= '3'  ); // => true
console.log( 2   >=  3   ); // => false
console.log( '7' >=  9   ); // => false

小于运算符 (<)

使用小于运算符（<）比较两个数字的大小。如果小于运算符左边的数字比右边的数字小，它会返回 true，否则会返回false。

语法示例如下所示：

x < y

与相等运算符类似，小于运算符在做比较的时候会转换值的数据类型。

例如

console.log( 3   < 5   ); // => true
console.log( '4' < 7   ); // => true
console.log( 6   < 5   ); // => false
console.log( 8   < 2   ); // => false
console.log( '6' < 4   ); // => false

小于等于运算符 (<=)

使用小于等于运算符（<=）比较两个数字的大小。如果在小于等于运算符左边的数字小于或者等于右边的数字，它会返回 true。如果在小于等于运算符左边的数字大于右边的数字，它会返回 false。

语法示例如下所示：

x <= y

与相等运算符类似，小于等于运算符会转换数据类型。

例如

console.log( 2   <= 5   ); // => true
console.log( '7' <= 7   ); // => true
console.log( 5   <= 5   ); // => true
console.log( 8   <= 2   ); // => false
console.log( '7' <= 4   ); // => false

定义函数 testComparison ，通过参数 val 进行数值比较，学习4种比较运算符的使用。条件语句中 val > 10 && val < 13  比较特殊，会以后会文章中介绍逻辑与操作。

function testComparison(val) {
  if (val >= 18) { 
    return "大于等于18";
  }

  if ( val > 10 && val < 13 ) { 
    return "小于13大于8";
  }

  if (val > 8){
    return "大于8";
  }

  if (val <= 8){
    return "小于等于8";
  }
  return "不匹配";
}

console.log(testComparison(18)); // => 大于等于18
console.log(testComparison(13)); // => 大于8
console.log(testComparison(11)); // => 小于13大于8
console.log(testComparison(8)); // => 小于等于8

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
