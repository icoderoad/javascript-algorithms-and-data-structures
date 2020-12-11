---
id: 5fd30e68f91e702ce0ce8e40
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 switch 语句从多个选项中进行选择及设置默认选项
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用 switch 语句从多个选项中进行选择及设置默认选项。

如果你有非常多的选项需要选择，可以使用 switch 语句进行条件选择。根据不同的参数值会匹配上不同的 case 分支，语句会从第一个匹配的 case 分支开始执行，直到碰到 break 语句就结束执行。

语法示例如下所示：

switch (表达式) {
  case 条件值1:
    // 当 表达式 的结果与 条件值1 匹配时，从此处开始执行
    执行代码块1；
    [break;]
  case 条件值2:
    // 当 表达式 的结果与 条件值2 匹配时，从此处开始执行
    执行代码块2;
    [break;]
  ...
  case 条件值N:
    // 当 表达式 的结果与 条件值N 匹配时，从此处开始执行
    执行代码块N;
    [break;]
  default:
    // 如果 表达式 与上面的 条件值 值都不匹配时，执行默认代码块
    执行代码块_默认;
    [break;]
}

为了熟悉 switch 语句如何使用，我们可以写一个获取中文星期的函数 getWeekDayName, 示例代码如下所示：

function getWeekDayName( day ){
  var dayName = "";
  switch( day ){
    case 0 :
      dayName = "星期日";
      break;
    case 1 :
      dayName = "星期一";
      break;
    case 2 :
      dayName = "星期二";
      break;
    case 3 :
      dayName = "星期三";
      break;
    case 4 :
      dayName = "星期四";
      break;
    case 5 :
      dayName = "星期五";
      break;
    case 6 :
      dayName = "星期六";
      break;
    default:
      dayName = "参数错误";
      break;
  }
  return dayName;
}

console.log( getWeekDayName( 0 ) ); // => 星期日
console.log( getWeekDayName( 6 ) ); // => 星期六
console.log( getWeekDayName( 8 ) ); // => 参数错误

以上函数代码通过参数 day 的不同值返回不同的星期名称，有效值为 0-6，如果不能匹配 0-6 条件值，返回默认值 “参数错误”。 

注意：switch 语句在比较值时使用的是全等操作符，因此不会发生类型转换。

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
