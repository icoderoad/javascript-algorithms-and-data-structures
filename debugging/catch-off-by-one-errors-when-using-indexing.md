---
id: 602861e24d084c518a8e40ac
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 捕获使用索引的时候出现的错误

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/debuging.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

捕获使用索引的时候出现的错误

当试图访问字符串或数组的特定索引（分割或访问一个片段）或循环索引时，有时会出现 Off by one errors 错误（有时称为 大小差一或OBOE）。大小差一就是指某个变量的最大值和最小值可能会和正常值差 1，或者循环多执行一次或少执行一次，一般在临界情况时发生。

JavaScript 语言索引从 0 开始，而不是 1，这意味着最后一个索引总会比字符串或数组的长度少 1。如果尝试访问等于长度的索引，程序可能会抛出“索引超出范围”引用错误或打印出 undefined。

当使用将索引范围作为参数的字符串或数组方法时，阅读相关的文档并了解参数中的索引的包含性（即是否考虑进返回值中）很重要。以下是一些错误的示例：

let alphabet = "abcdefghijklmnopqrstuvwxyz";
let len = alphabet.length;
for (let i = 0; i <= len; i++) {
  // 在最后多了一次循环
  console.log( alphabet[i] );
}

for (let j = 1; j < len; j++) {
  // 循环少了一次，漏掉了索引 0 处的字符
  console.log( alphabet[j] );
}

for (let k = 0; k < len; k++) {
  // 不多不少，这才是正确的
  console.log( alphabet[k] );
}

以上代码在控制台执行，第一个循环执行后，执行到最后一次循环时，由于索引值超出了字符串长度，执行结果返回 undefined。第 2 个循环由于从 1 开始执行，控制台打印的执行结果少了字母 a，控制台打印的结果是从 b 到 z。第三个循环正确输出从 a 到 z 的所有字符。注意第 3 个正确循环的变量 k 的条件设置，变量 k 从 0 开始，结束条件是循环变量小于字符串长度，不包括字符串长度。


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
