---
id: 6008e61491b0e1d06a048e84
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 正则匹配时忽略大小写
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

正则匹配时忽略大小写

到目前为止，我们已经了解了如何用正则表达式来执行字符串的匹配。但有时候，并不关注匹配字母的大小写。

大小写即大写字母和小写字母。大写字母如 "A"、"B" 和 "C"。小写字母如 "a"、"b" 和 "c"。

可以使用可选参数（flags）来匹配这两种情况。可选参数有很多，不过这里我们只关注忽略大小写的可选参数 ——i。可以通过将它附加到正则表达式之后来使用它。这里给出使用该可选参数的一个实例 /icoderoad/i 。这个字符串可以匹配字符串 "icoderoad"、"iCoderoad" 和 "iCodeRoad"。

下面我们做个练习，编写正则表达式 strRegex 以匹配 "iCodeRoad"，忽略大小写。正则表达式不应与任何缩写或带有空格的变体匹配,具体偌。

let myString = "您好, 编程小白。路条编程(www.iCodeRoad.com)欢迎您！";
let strRegex = /icoderoad/i; 
let result = strRegex.test(myString);
console.log(result);
// => true
myString = "您好, 编程小白。路条编程(www.iCRoad.com)欢迎您！";
result = strRegex.test(myString);
console.log(result);
// => false

myString = "您好, 编程小白。路条编程(www.iCode Road.com)欢迎您！";
result = strRegex.test(myString);
console.log(result);
// => false

以上代码在控制台执行后，可以匹配 忽略大小写的"iCodeRoad"，不与任何缩写或带有空格的变体匹配，控制分别输出 
true 
false
false
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
