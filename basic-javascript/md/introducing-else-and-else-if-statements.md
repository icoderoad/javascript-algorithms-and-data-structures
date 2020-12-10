---
id: 5fd1b3ebf3b42a54564b29e3
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: else 和 else if 语句介绍
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
else 和 else if 语句介绍。

前面文章中我们介绍过 if 条件语句，当 if 语句的条件为真时，执行大括号里的代码，那如果条件为假呢？正常情况下什么也不会发生。使用 else 语句，可以执行当条件为假时相应的代码。示例代码如下所示

function  checkIfAdult( age ){
  if (age >= 18) {
    return "已成年";
  } else {
    return "未成年";
  }
}

console.log( checkIfAdult(8)  ); // => 未成年
console.log( checkIfAdult(18)  ); // => 已成年

以上代码定义了根据年龄参数判断是否成年的函数 checkIfAdult， 通过设置参数为 8， 18 调用函数 checkIfAdult， 在控制台打印相应状态。 参数为 8 时，控制台输出未成功， 参数为 18 时， 控制台输出已成年。


如果你有多个条件语句，你可以通过 else if 语句联合 if 语句一起使用。

语法如下所示：

if (条件1)
   语句1
else if (条件2)
   语句1
else if (条件3)
   语句1
...
else
   语句N


假如我们要实现一个通过一个标识参数 status 的不同值获取用户状态描述的函数 getUserStatus, 通过 if 和 else if 语句实现代码如下所示：

function getUserStatus ( status ){
  if( status ==='normal' ){ 
      return  "正常";
  }else if( status ==='unactive'  ){
      return  "未激活";
  }else if( status ==='locked'  ){
      return  "锁定";
  }else if( status ==='del'  ){
      return  "删除";
  }else{
      return  "未知";
  }
}

console.log( getUserStatus( 'normal' ) ); // => 正常
console.log( getUserStatus( 'del' ) ); // => 删除

以上代码实现的是通过 status 参数值，返回中文描述的函数 getUserStatus， 如果不能满足所有if 和 else if 条件，返回未知状态。

if、else if 语句中代码的执行顺序是很重要的，上面示例的代码与代码顺序关系不大。有些情况下，在条件语句中，代码的执行结果与输写代码的顺序有很大关系。条件语句代码的执行顺序是从上到下，所以你需要考虑清楚先执行哪一句，后执行哪一句，这有两个例子，大家可以比较下程序的输出结果区别。

第一个例子：

function checkNum(num) {
  if (num < 1) {
    return "小于1";
  } else if (num < 2) {
    return "小于2";
  } else {
    return "大于或等于2";
  }
}

第二个例子更改了代码的执行顺序：

function checkNum2(num) {
  if (num < 2) {
    return "小于2";
  } else if (num < 1) {
    return "小于1";
  } else {
    return "大于或等于2";
  }
}

这两个函数看起来几乎一模一样，我们传一个值进去看看它们有什么区别。在控制台调用两个函数，参数值都传 0, 大家可以比较下执行结果。

console.log( checkNum(0) ); // => 小于1
console.log( checkNum2(0) ); // => 小于2

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
