---
id: 5fcb4f1e3970974fddc9debc
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 布尔值及 if 条件逻辑语句
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
布尔值及 if 条件逻辑语句。

JavaScript 语言中另一种数据类型是布尔（Boolean）。布尔值要么是 true 要么是 false 。它非常像电路开关，true 是 “开”，false 是 “关”，这两种状态是互斥的。

下面的所有的代码行均会创建初始值为 false 的 Boolean 对象。

var flag = new Boolean();
var flag = new Boolean(0);
var flag = new Boolean(null);
var flag = new Boolean("");
var flag = new Boolean(false);// 不带单引号的是 false
var flag = new Boolean(undefined);
var flag = new Boolean(NaN);

下面的所有的代码行均会创初始值为 true 的 Boolean 对象：
var flag = new Boolean(1);
var flag = new Boolean(true);
var flag = new Boolean("true");
var flag = new Boolean("false");//带单引号的字符串false最终等于true
var flag = new Boolean("Bill Gates");

0、null、""、false、undefined 或 NaN，这些都可以自动转化为布尔值的 false，其他值都为 true（即使当变量值为字符串 "false" 时也为 true）！

注意：布尔值是不带引号的，"true" 和 "false" 是字符串而不是布尔值，在 JavaScript 语言中也没有特殊含义。


if 语句用于在代码中做条件判断。关键字 if 告诉 JavaScript 语言在小括号中的条件为真的情况下去执行定义在大括号里面的代码。这种条件被称为 Boolean 条件，因为他们只可能是 true（真）或 false（假）。

当条件的计算结果为 true，程序执行大括号内的语句。当布尔条件的计算结果为 false，大括号内的代码将不会执行。

if (condition){
  statement
}

参数说明：
condition ： 值为真或假的表达式
statement ：当 condition 为真时执行的语句。可为任意语句，包括更深层的内部if语句。要执行多条语句，使用块语句（{ ... }）将这些语句分组；若不想执行语句，则使用空语句。 

if 条件语句代码示例如下所示：

function isAdult (age) {
   var isAdult = age >=18 ? true : false ;
  if (isAdult) {
     return "已成年";
  }
  return "未成年";
}
console.log( isAdult(18) );  // => 已成年
console.log( isAdult(14) ); // => 未成年
  
以上代码定义了一个根据年龄验证是否成年的函数， 如果大于等于18周岁则为成年，否则为未成功。函数中第一行使用了三元运算符，具体用法会在后面的文章中详细介绍。
函数下面是两个控制台日志语句，第一条调用 isAdult 函数， 参数值为 18 ，控制台输出 ”已成年“ ，第二条语句参数值为 14 ，控制台输出 “未成年”。

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
