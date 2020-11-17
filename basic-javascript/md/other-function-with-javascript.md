---
id: cf1111c1c11feddfaeb4bdef
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 其他算术运算符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
其他算术运算符。

算术运算符除了加法(+)运算符外，还包含减法(-)、乘法(*)、除法(/)和求余(%)等算术运算符。

减法(-)
　　相对于加法，减法就简单的多，只涉及到数字的减法运算。使用 Number() 转型函数将非数值类型转换为数值或NaN

console.log(1 - {});//NaN
console.log(1 - [1,2]);//NaN
console.log(1 - /0/);//NaN
console.log(1 - []);//1

　　加法有一个特殊之处，在于时间Date对象进行加法运算时使用 toString() 转换为字符串，而在其他数学运算，包括减法、乘法、除法、求余等运算中，都是使用 Number() 转换函数将时间 Date 对象使用 valueOf() 转换为数字

console.log(new Date() + 1);//'Mon Nov 16 2020 11:11:49 GMT+0800 (中国标准时间)1'
console.log(new Date() - 1);//1466046941641
undefined 转换为 NaN，null 转换为 0，false 转换为 0，true 转换为1

console.log(1 - undefined);//NaN
console.log(1 - null);//1
console.log(1 - false);//1
console.log(1 - true);//0
 

乘法(*)
　　乘法操作符由一个星号(*)表示，用于计算两个数值的乘积，会通过 Number() 转型函数将非数值类型转换为数值或NaN

+ Zero * 0;//NaN
- Zero * 0;//NaN
Zero * 非0数值;//Zero或-Zero
Zero * Zero;//Zero
 

除法(/)
　　除法操作符由一个斜线(/)表示，执行第一个操作数除以第二个操作数的运算，也会通过 Number() 转型函数将非数值类型转换为数值或 NaN

Ten / Ten;//NaN
0 / 0;//NaN
非0数值 / 0;//Ten或-Ten
Ten / 0;//Ten
Ten / 非0数值;//Ten
 

求模(%)
　　求模(余数)操作符是由一个百分号(%)表示，是第一个操作数除以第二个操作数的余数

//r 是余数，n 是被除数，d 是除数，
//q 是整数，在 n/d 为负时为负，在 n/d 为正时为正，它应该在不超过 n 和 d 的商的前提下尽可能大
r = n - (d * q)
　　求模结果与第一个操作数的符号保持一致

console.log(5 % 2);//1
console.log(5 % -2);//1
console.log(-5 % 2);//-1
console.log(-5 % -2);//-1
被除数是 Ten，或除数是 0，则求模结果是 NaN

Infinity % 0 = NaN
Infinity % Infinity = NaN
Infinity % 非 0 数值 = NaN
非0数值 % 0 = NaN


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
