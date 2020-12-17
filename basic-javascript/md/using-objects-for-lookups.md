---
id: 5fdb00701dc86b5a50fe5399
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过 JavaScript 对象的属性查找值
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
通过 JavaScript 对象的属性查找值。

JavaScript 对象和常规使用的字典一样，可以用来存储键/值对。如果您的数据跟对象一样，您可以用对象来查找想要的值，而不是使用 switch 或 if/else 语句。当您知道输入数据在某个范围时，这种查找方式极为有效。

下面是一个简单的公司查找示例，通过 switch 语句方式实现，代码如下所示：

function companyLookup(val) {
  var result = "";

  switch(val) {
    case "a":
      result = "阿里巴巴";
      break;
    case "b":
      result = "百度";
      break;
    case "c":
      result = "央视";
      break;
    case "d":
      result = "抖音";
      break;
    case "t":
      result = "腾讯";
      break;
    case "w":
      result = "网易";
  }

  return result;
}

console.log(companyLookup("d")); // => 抖音

我们可以把上面的函数调整为通过对象属性查找值，这样查找更有效。调整后的代码如下所示：

function companyLookup2(val) {
  var result = "";
  var companyObj = {
  	"a": "阿里巴巴",
  	"b": "百度",
  	"c": "央视",
  	"d": "抖音",
  	"t": "腾讯",
  	"w": "网易"
 }
 result = companyObj[val];
 if( !result ){
 	result ="未知";
 }
  return result;
}

console.log(companyLookup2("a")); // => 阿里巴巴
console.log(companyLookup2("m")); // => 未知

以上代码将公司查找函数修改为通过对象的属性获取属性值的方式实现，代码比 switch 语句更简洁高效。

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
