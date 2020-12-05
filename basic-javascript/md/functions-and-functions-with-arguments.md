---
id: 5fc7700d855bd456bb1cbad4
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:	用函数编写可复用代码及将值传递给带参函数
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
用函数编写可复用代码及将值传递给带参函数。

在 JavaScript 语言中，我们可以把代码的重复部分抽取出来，放到一个函数中。

函数是 JavaScript 语言中的基本组件之一。 一个函数是 JavaScript 语言的过程 —-- 一组执行任务或计算值的语句。要使用一个函数，必须将其定义在希望调用它的作用域内。

一个 JavaScript 函数用 function 关键字定义，后面跟着函数名和圆括号。
一个函数定义也称为函数声明或函数语句，由一系列的 function 关键字组成，依次为：
函数的名称
函数参数列表，包围在括号中并由逗号分隔
定义函数的 JavaScript 语句，用大括号 {} 括起来

例如，以下的代码定义了一个简单的 helloMsg 函数：

function helloMsg(){
  console.log("Hello World");
}

你可以通过函数名 helloMsg 加上后面的小括号来调用这个函数，就像这样： helloMsg(); 每次调用函数时，它都会在控制台上打印消息"Hello World"。每次调用函数时，大括号之间的所有代码都将被执行。

函数的参数列表在函数中充当占位符(也叫形参)的作用，参数可以为一个或多个。调用一个函数时所传入的参数为实参，实参决定着形参真正的值。简单理解：形参即形式、实参即内容。

将 helloMsg 函数调整为带有两个参数的函数，param1 和 param2，调整后的参数代码如下所示：

function helloMsg(param1, param2) {
  console.log(param1, param2);
}

接着我们调用 helloMsg 函数： helloMsg("Hello", "World"); 我们传递了两个参数，"Hello" 和 "World" 。在函数内部，param1 等于 “Hello” ，param2 等于 “World”。

 helloMsg("Hello", "World"); // => Hello World
 helloMsg("Welcome to ", "Beijing！"); // => Welcome to  Beijing！
 
注意：helloMsg 函数可以多次调用，每次调用时传递的参数会决定形参的实际值。


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
