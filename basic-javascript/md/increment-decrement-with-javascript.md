---
id: 56533eb9ac21ba0edf2244ac
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 算术运算符递增和递减
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
算术运算符递增和递减。

JavaScript 语言中的递增和递减运算符都是一元操作符，言外之意就是只能操作一个值的操作符。递增和递减操作符直接借鉴自 C 语言，各有两种版本：前置型(递增 ++i，递减 --i )和后置型(递增 i++，递减 i-- )。

在 JavaScript 语言中，递增（递减）的前置和后置运算符对于初学者都非常容易混淆。希望通过本文章的学习，将这两者的使用和不同之处了解清楚。

前置型递增(递减)：
前置型递增也称之为前增量( pre-increment )运算符，它对操作数进行增量计算，并返回其计算后的值。简单说就是先自身计算，再赋值给变量。假设有一个变量 i，其值为 3。那么前置递增为 ++i。

var i = 3;
console.log(i); // => 3
++i;
console.log(i); // => 4

这个示例，前置递增 ++i 操作符把 i 的值变成了4(也就是 3+1 )。实际上，执行前置递增 ++i 和执行下面的表达式效果相同：

var i = 3;
i = i + 1;
console.log(i); // => 4

简单点讲，前置型递增就是先自身计算，再赋值给变量：

var i = 3;
var a = ++i;  // var i = 3; i = i + 1; a = i;
console.log(a); // => 4
console.log(i); // => 4

其中 var a = ++i ,实际上做了下面这几个操作：

i = 3 ;
a = i + 1;
i = i + 1;
a = i;

前置递减 --i 和前置递增 ++i 类似，不同的是先做减法(减 1 )，再赋值。比如:

var i = 8;
a = --i;
console.log(a); // => 7
console.log(i); // => 7

代码中的 --i 相当于：

var i =  8 ;
i = i - 1;
a = i - 1;
a = i;

执行前置递增和递减时，变量的值都是在语句被求值以前改变的(返回它递增(减)之后的值)。来看个例子：

var num = 38;
var anotherNum = --num + 2;
console.log(num) // => 37 (num = num - 1)
console.log(anotherNum); // 39 (anotherNum = num - 1 + 2)

这个示列中变量 anotherNum 的初始值等于变量 num 的值前置递减 (num = num - 1) 再加上 2。也就是前置 --num 先做减法操作，num的值变成了 37，所以再加上 2，其值就是 39。


后置型 (递增 i++ ，递减 i-- )：先将自身的值赋值给变量，然后再自身计算


假设变量 i=88 ，那么后置递增为 i++ 。

 var i = 88;
 console.log( i ）; // =>  88 　　　　　　　　
 i++;　//　　 => 88 　　　　     
 console.log( i ); // => 89     

把递增操作符放在变量后面并不会改变语句的结果，因为递增是这条语句的唯一操作。但是当语句中还包含其他操作时，区别就不一样了。看下面的例子：

var num1 = 2;
var num2 = 20;
var num3 = num1++  +  num2;
var num4 = num1 + num2;
console.log(num1); // =>  3  
console.log(num3); // =>  22  
console.log(num4); // =>  23 

总结：前置递增(递减)和后置递增(递减)
1.前置递增（++）： 在变量的前面，先自身执行加法操作后再赋值(++i)

2.后置递增（++）： 在变量的后面，先赋值后再执行加法操作(i++)

3.前置递减（--）： 在变量的前面，先自身执行减法操作后再赋值(--i)

4.后置递减（--）： 在变量的前面，先赋值后再执行减法操作(i--)

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
