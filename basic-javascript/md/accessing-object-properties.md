---
id: 5fd8719eaec7b4e002e4faf0
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过点符号及中括号访问对象属性
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
通过点符号及中括号访问对象属性。

在JavaScript 语言中，有两种方式访问对象属性，一种是点操作符(.)，另一种是中括号操作符([])。

第一种当你知道所要读取的属性的名称的时候，使用点操作符访问对象属性值。

以前面介绍的 dog 对象为例

var dog = {
  "name": "小花",
  "legs": 4,
  "tails": 1,
  "color": "black"
};

使用点操作符读取 dog 对象属性的示例如下所示：

var name = dog.name;  
var color = dog.color; 
console.log( name ); // => 小花
console.log( color ); // => black

以上代码通过对象名称 dog 及点操作符访问对应属性名称 name，color，将属性值赋值给变量 name 和 color ,在控制台输出对应变量的值分别为"小花"和"black"。

第二种访问对象属性的方式是通过中括号操作符([])访问对象属性值，如果你想访问的属性的名称有一个空格，这时你只能使用中括号操作符([])。

当然，如果属性名不包含空格，也可以使用中括号操作符。

这是一个使用中括号操作符([])读取对象属性的例子：

var userObj = {
  "first Name": "国藩",
  "last Name": "曾",
  "Style oneself as": "涤生"
};

console.log(userObj["first Name"]); // => 国藩
console.log(userObj["last Name"]); // => 曾
console.log(userObj["Style oneself as"]); // => 涤生

提示：属性名称中如果有空格，必须把属性名称用单引号或双引号包裹起来。

中括号操作符的另一个使用方式是访问赋值给变量的属性。当你需要遍历对象的属性列表时，这种方式极为有用。

我们继续拿 userObj 对象为例，通过一个变量 name 来访问属性"irst Name"的例子代码如下所示：

var name = "first Name";
var nameVal = userObj[name];
console.log( nameVal ); // => 国藩


使用此概念的另一种方法是在程序执行期间动态收集属性名称，如下所示：

var userObj2 = {
  propName: "曾国藩"
};

function concatProp(str) {
  var s = "prop";
  return s + str;
}
var strProp = concatProp("Name"); 
console.log(userObj2[strProp]); // => 曾国藩

提示：当我们通过变量名访问属性的时候，不需要给变量名包裹引号。因为实际上我们使用的是变量的值，而不是变量的名称。

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
