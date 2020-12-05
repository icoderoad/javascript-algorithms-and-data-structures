---
id: 5fc8a5f554d88dc8627ea433
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:	全局、局部作用域和函数中的全局作用域及局部作用域
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
全局、局部作用域和函数中的全局作用域及局部作用域。

在 JavaScript 语言中，作用域涉及到变量的作用范围。在函数外定义的变量具有全局作用域。这意味着，具有全局作用域的变量可以在代码的任何地方被调用。

这些没有使用 var 关键字定义的变量，会被自动创建在全局作用域中，形成全局变量。当在代码其他地方无意间定义了一个变量，刚好变量名与全局变量相同，这时会产生意想不到的后果。因此你应该总是使用 var 关键字来声明你的变量。

在一个函数内声明的变量，以及该函数的参数都是局部变量，意味着它们只在该函数内可见。

在函数外声明一个全局变量 myGlobal ，并给它一个初始值 10。在函数 fun1 的内部，不使用 var 关键字来声明 oopsGlobal，并赋值为 5。

var myGlobal = 10;
function fun1() {
  oopsGlobal = 5;
}


function fun2() {
  var output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}

fun2(); // =>  myGlobal: 10

以上代码在控制台执行后，控制台输出 myGlobal: 10， 说明变量 myGlobal 为全局变量 ， oopsGlobal 变量即使没有使用 var 关键字声明，也为局部变量。

一个程序中有可能具有相同名称的局部变量和全局变量。在这种情况下，局部变量将会优先于全局变量。

以下面代码为例：

var strCity = "北京";
function myFun() {
  var strCity = "上海";
  return strCity;
}

myFun(); // => "上海"

调用函数 myFun 将会在控制台输出 "上海"，因为局部变量优先级更高。

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
