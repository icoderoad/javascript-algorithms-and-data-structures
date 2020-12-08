---
id: 5fcdbec6415fbb8f0be2883c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 不等与严格不等运算符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
不等与严格不等运算符。

不等运算符（!=）与相等运算符是相反的。这意味着不相等运算符中，如果“不为真”并且返回 false 的地方，在相等运算符中会返回 true ，反之亦然。与相等运算符类似，不相等运算符在比较的时候也会转换值的数据类型。

语法如下所示：

x != y

示例如下所示：

console.log( 1 !=   2 ) ; // => true
console.log( 1 !=  "1" ) ;   // => false
console.log( 1 !=  '1' ) ;   // => false
console.log( 1 !=  true ) ;  // =>  false
console.log( 0 !=  false ) ; // =>  false


严格不等运算符（!==）与严格相等运算符是相反的。这意味着严格不等并返回 false 的地方，用严格相等运算符会返回 true，反之亦然。严格不等运算符不会转换值的数据类型。
语法如下所示：

x !== y

示例如下所示：

console.log( 3 !==  3  ) ; // => false
console.log( 3 !== '3' ) ; // => true
console.log( 4 !==  3  ) ; // => true

在下面的代码示例中，将函数 testStrictNotEqual 中的 if 语句设置为严格不等运算符 !==，如果 val 与 88 严格不等的时候，函数会返回 "不等"，否则返回 “相等”。

function testStrictNotEqual(val) {
  if (val !== 88 ) {
    return "不等";
  }
  return "相等";
}

console.log( testStrictNotEqual(10) ); // => 不等
console.log( testStrictNotEqual(88) ); // => 相等


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
