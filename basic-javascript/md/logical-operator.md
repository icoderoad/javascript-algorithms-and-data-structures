---
id: 5fd08d3dc5d1febe39462cc2
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 逻辑运算符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
逻辑运算符。

在 JavaScript 语言中，常用逻辑运算符分为逻辑与(&&)、逻辑或(||)，两种运算符的返回值都是布尔值。

逻辑与(&&)

语法示例如下所示：

表达式1 && 表达式2

如果 表达式1 可以转换为 true，则返回 表达式2; 否则， 返回 表达式1 。

有时你需要在一次判断中做多个操作。当且仅当运算符的左边和右边都是 true，逻辑与运算符（&&）才会返回 true。

只有当 num 的值在 6 和 9 之间（包括 6 和 9）才会返回 "正常"。相同的逻辑可被写为以下 checkNum 函数：

function checkNum( num ) {
  if (num > 5 && num < 10) {
    return "正常";
  }
  return "异常";
}
console.log(checkNum(8)); // => 正常
console.log(checkNum(13));  // => 异常

同样的效果可以通过 if 语句的嵌套来实现：

function checkNum( num ) {
  if (num > 5) {
    if (num < 10) {
      return "正常";
    }
  }
  return "异常";
}
console.log(checkNum(8)); // => 正常
console.log(checkNum(13));  // => 异常

逻辑或(||)

语法示例如下所示：

表达式1 || 表达式2

逻辑或运算符由两个管道符号（|）组成。这个按键位于退格键和回车键之间。逻辑或(||) 和逻辑与 (&&) 的操作类似，只要逻辑或运算符 || 两边任何一个为 true，那么它就返回 true，否则返回 false 。

注意：当第一个表达式求值为 false，但第二个表达式未定义时，会报错。

再以验证数字的函数为例，如果数字介于 5 至 10 之间，返回正常，否则返回异常，常规条件语句函数如下所示：

function checkNum( num ){
  if (num > 10) {
    return "异常";
  }
  if (num < 5) {
    return "异常";
  }
  return "正常";
}
console.log(checkNum(18)); // => 异常
console.log(checkNum(7)); // => 正常

相同的逻辑可以通过逻辑或(||)简写成如下函数：

function checkNum( num ){
  if (num > 10 || num < 5) {
    return "异常";
  }
  return "正常";
}
console.log(checkNum(18)); // => 异常
console.log(checkNum(7)); // => 正常



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
