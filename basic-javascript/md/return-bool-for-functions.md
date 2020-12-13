---
id: 5fd570fb59f4cadffe38ab28
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 函数中的 rturn 语句用法及如何返回布尔值
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
函数中的 rturn 语句用法及如何返回布尔值。

前面文章中的示例函数中都有 return 语句，当代码执行到 return 语句时，函数返回结果就结束运行函数，return 后面的语句不会执行。

定义一个测试返回 return 语句的函数 testReturn，示例代码如下所示：

function testReturn() {
  console.log("天行健");
  return "君子以自强不息";
  console.log("地势坤，君子以厚德载物")
}

testReturn(); 

上面的代码在控制台输出"天行健"、返回 "君子以自强不息"，但没有输出"地势坤，君子以厚德载物"，因为函数遇到 return 语句就提前结束了。

到现在为止，我们介绍的函数都是返回字符串的，如果我们想通过返回布尔类型的，应该如何操作呢？在相等运算符的文章中我们提到所有比较操作符都会返回 boolean 类型，要么是 true 要么是 false。

以比较两个数是否相等为例，通过 if/else 语句来做比较然后返回 true 或 false，代码如下所示：

function isEqual(val1, val2) {
  if (val1 === val2) {
    return true;
  } else {
    return false;
  }
}

有一个更好的方法，因为 === 总是返回 true 或 false，所以我们可以直接返回比较的结果：

function isEqual(val1, val2) {
  return val1 === val2;
}

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
