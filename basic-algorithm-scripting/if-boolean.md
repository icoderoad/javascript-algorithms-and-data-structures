---
id: 604ef093e49cf062c9f7fd0c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 检查参数是否为布尔类型
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

检查参数是否为布尔类型

今天我们介绍检查参数是否为布尔类型的方法。检查参数是否为布尔类型。是则返回 true ，否则返回 false。在介绍具体方法之前，我们先介绍下 typeof 操作符的用法。

typeof 操作符返回一个字符串，表示未经计算的操作数的类型。

语法：

typeof 运算符后接操作数：

typeof operand

typeof(operand)

参数：

operand

一个表示对象或原始值的表达式，其类型将被返回。

描述

下表总结了 typeof 可能的返回值。有关类型和原始值的更多信息，可查看 JavaScript 数据结构 页面。

类型                              结果
Undefined                     "undefined"
Null                          "object" (见下文)
Boolean                       "boolean"
Number                        "number"
BigInt(ECMAScript 2020 新增)   "bigint"
String                        "string"
Symbol (ECMAScript 2015 新增) "symbol"
Function 对象 (按照 ECMA-262 规范实现 [[Call]]) "function"
其他任何对象                    "object"

实现步骤如下所示：

1、通过 typeof 操作符获取参数类型字符串并赋值给一个新变量

2、对新变量与布尔字符串值 “boolean” 进行比较

3、比较值如果为真返回 true , 否则返回 false  

具体代码实现方法如下：

function checkBoolVar( param ) {

 var typeVal = typeof param;
 if( typeVal === "boolean" ) {
   return true;
 }else{
   return false;
 }

}

console.log( checkBoolVar(true) );
// => true

console.log( checkBoolVar("false") );
// => false

console.log( checkBoolVar(['www','icoderoad', 'com']) );
// => false


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
