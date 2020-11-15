---
id: 56533eb9ac21ba0edf2244aa
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 理解未初始化的变量
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
理解未初始化的变量。

当 JavaScript 中的变量被声明的时候，程序内部会给它一个初始值 undefined 。当你对一个值为 undefined 的变量进行运算操作的时候，算出来的结果将会是 NaN，NaN 的意思是 "Not a Number" 。当你用一个值为 undefined 的变量来做字符串拼接操作的时候，它会输出字符串 "undefined" 。

undefined 表示"缺少值"，就是此处应该有一个值，但是还没有定义。典型用法是：

（1）变量被声明了，但没有赋值时，就等于 undefined。

（2) 调用函数时，应该提供的参数没有提供，该参数等于 undefined。

（3）对象没有赋值的属性，该属性的值为 undefined。

（4）函数没有返回值时，默认返回 undefined。

用法 2-4部分我们会在后继文章中进行介绍。

通常在声明变量的时候会给变量初始化一个初始值, 如下代码所示：

var myVar = 0;

以上代码创建了一个名为 myVar 的变量并指定一个初始值为 0 。

如果只定义变量，不给变量初始化初始值，myVar 变量的值就是 undefined。

定义 3 个变量 a、b、c，并且分别给他们赋值：5、10、"I am a"，这样它们值就不会是 undefined 了。代码示例如下所示：

var a = 5;
var b = 10;
var c = "I am a";

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
