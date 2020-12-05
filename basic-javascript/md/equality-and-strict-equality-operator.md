---
id: 5fcc155a21d521d3fdf361af
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 相等与严格相等运算符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
相等与严格相等运算符。

JavaScript 语言中提供两种相等运算符：相等(==)和严格相等(===)。简单说，它们的区别是相等运算符（==）比较两个值是否相等，严格相等运算符（===）比较它们是否为“同一个值”。如果两个值不是同一类型，严格相等运算符（===）直接返回 false，而相等运算符（==）会将它们转换成同一个类型，再用严格相等运算符进行比较。

最基本的运算符是相等运算符：== 。相等运算符比较两个值，如果它们相等，返回 true，如果它们不等，返回 false。

注意：相等运算符不同于赋值运算符（=），赋值运算符是把等号右边的值赋给左边的变量。

function checkEqual(val1, val2) {
  if (val1 == val2) {
     return "相等";
  }
  return "不等";
}

console.log( checkEqual(1, "1" ) ); // => 相等
console.log( checkEqual(false, "false" )  ); // => 不等
console.log( checkEqual(1, 8 ) ); // => 不等
console.log( checkEqual("路条编程", "编程路条" )  ); // => 不等

以上代码中，如果 val1 与 val2 相等,相等运算符会返回 true，因此大括号里面的代码会被执行，函数将返回 "相等"。否则，函数返回 "不等"。 在 JavaScript 语言中，为了让两个不同的数据类型（例如数字和字符串）的值可以作比较，它必须把一种类型转换为另一种类型。类似上面控制台的第一行和第二行代码，必须要强制进行类型转换后再进行比较。

严格相等运算符（===）是相对相等操作符（==）的另一种比较操作符。与相等操作符不同的是，它会同时比较元素的值和数据类型。

如果比较的值类型不同，那么在严格相等运算符比较下它们是不相等的，会返回 false 。重写函数为严格相等比较，代码如下所示：

function strictCheckEqual(val1, val2) {
  if (val1 === val2) {
     return "相等";
  }
  return "不等";
}

console.log( strictCheckEqual(1, "1" ) ); // => 不等
console.log( strictCheckEqual(false, "false" )  ); // => 不等
console.log( strictCheckEqual(8, 8 )  ); // => 相等

以上代码中，如果 val1 与 val2 相等并且值类型相同, 严格相等运算符会返回 true ，因此大括号里面的代码会被执行，函数将返回 "相等"，否则，函数返回 "不等"。


## Instructions
<section id='instructions'>

</section>

## Tests
<section id='tests'>
函数一般用return语句来返回值，但这不是必须的。在函数没有return语句的情况下，当你调用它时，该函数会执行内部代码，返回的值是undefined。

示例

var sum = 0;
function addSum(num) {
  sum = sum + num;
}
addSum(3); // sum will be modified but returned value is undefined
addSum是一个没有return语句的函数。该函数将更改全局变量sum，函数的返回值为undefined。



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
