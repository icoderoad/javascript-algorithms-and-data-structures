---
id: 5fe7cf65082e9007a79e7043
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 三元运算符用法详解
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
三元运算符用法详解。

三元运算符是 JavaScript 语言仅有的使用三个操作数的运算符。一个条件后面会跟一个问号（?），如果条件为真 ，则问号后面的 表达式A 将会执行；表达式A 后面跟着一个冒号（:），如果条件为假 ，则冒号后面的 表达式B 将会执行。本运算符经常作为 if 语句的简捷形式来使用。

语法：
条件表达式1 ？表达式2 ：表达式3

参数：

条件表达式1 是一个条件，值为 Boolean 类型
若 条件表达式1 的值为 true，则执行 表达式2 的操作，并且以 表达式2 的结果作为整个表达式的结果
若 条件表达式1 的值为 false，则执行 表达式3 的操作，并且以 表达式3 的结果作为整个表达式的结果

除了 false，可能的假值表达式还有：null 、NaN 、 0 、空字符串（ "" ）、和 undefined 。如果 条件表达式1 是以上中的任何一个, 那么条件表达式的结果就是 表达式3 执行的结果。

一般来说三元条件表达式与 if...else 语句有相同的表达效果，前者可以表达的后者同样也可以表达。两者最大的不同之处在于：if...else 是语句没有返回值，三元表达式有返回值。所以在需要返回值的场合，只能使用三元表达式，而不能使用 if...else 语句。

以一个学生考试成绩判断作为示例,条件如下：
如果成绩在 80 以上，则输出 优秀，如果成绩在 60 以上，则输出  合格，否则输出 不合格。

function getStudentAchievement( score ) {
    var result= score >= 80 ? "优秀" : (
        score >= 60 ? "合格" : "不合格");
    return result;
}
console.log( getStudentAchievement( 88 ) ); // => 优秀
console.log( getStudentAchievement( 66 ) ); // => 合格
console.log( getStudentAchievement( 55 ) ); // => 不合格

以上代码定义了一个根据学生分数获取考试成绩的函数 getStudentAchievement， 在控制台三次调用此函数，分数分别为 88、66、55，然后将结果在控制台输出，控制台的输出结果分别为 优秀、合格、不合格。

上面的示例使用的是一个三元运算符，您也可以将多个运算符串联在一起以检查多种条件。

下面的函数使用 if、else if 和 else 语句来检查多个条件，判断两个数字中相等或较大的数字：

function findGreaterOrEqual(a, b) {
  if (a === b) {
    return "a 和 b 相等";
  }
  else if (a > b) {
    return "a 和 b 两数中，a 大";
  }
  else {
    return "a 和 b 两数中，b 大";
  }
}

上面的函数使用三元运算符写法如下：

function findGreaterOrEqual(a, b) {
  return (a === b) ? "a 和 b 相等" 
    : (a > b) ? " a 和 b 两数中，a 大" 
    : " a 和 b 两数中，b 大";
}

即便如此，应谨慎使用多个三元运算符，因为在没有适当缩进的情况下使用多个三元运算符可能会使您的代码难以阅读。

例如下面代码：

function findGreaterOrEqual(a, b) {
  return (a === b) ? "a 和 b 相等" : (a > b) ? "a 和 b 两数中，a 大" : "a 和 b 两数中，b 大";
}

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
