---
id: 601f89eae45d68aed170ba10
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 程序调试简介
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

程序调试简介

调试对于程序员来说是一个有价值的必要的工具。它遵循测试阶段，即检查代码是否按预期工作，然后发现代码没有按预期工作的原因。调试是一个发现程序不起作用并修复它的过程。在花时间创建一个出色的代码块之后，很难意识到它可能有错误。这些问题通常有三种形式：

一、阻止程序运行的语法错误
二、代码无法执行或具有意外行为时出现运行时错误
三、当代码不按其本意运行时出现语义（或逻辑）错误

现代代码编辑器可以帮助识别语法错误。语义错误和运行时错误更难发现。它们可能导致您的程序崩溃，使其永远运行，或给出不正确的输出。把调试看作是试图理解代码为什么会以这种方式运行的一种方式。

语法错误示例-通常由代码编辑器检测到：

funtcion willNotWork( 
  console.log("Yuck");
}

上面代码中， “function” 关键字拼写错误，缺少括号。

下面是一个运行时错误的示例，此类问题通常在程序执行时检测到：

function loopy() {
  while(true) {
    console.log("Hello, world!");
  }
}

以上代码调用 loopy方法时， 会启动一个无限循环，这将会使您的浏览器崩溃。

下面是一个语义错误示例，此类问题通常在测试代码输出后检测到：

function calcAreaOfRect(w, h) {
  return w + h; // This should be w * h
}

let myRectArea = calcAreaOfRect(2, 3);

以上代码语法正确，程序可以正常执行，但程序执行后给出了错误的答案。

调试是令人沮丧的，但它有助于开发遵循一定的方法来审查您的代码。这意味着您可以从一个简单的过程开始，检查中间值和变量类型，看看它们是否和预期一致。

例如，如果函数 a 工作并返回它应该返回的内容，那么函数 B 可能有问题。或者从中间开始检查代码块中的值，尝试将搜索范围减半。一个点上的问题表示代码的前半部分有一个 bug。如果没有，很可能是在第二部分。


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
