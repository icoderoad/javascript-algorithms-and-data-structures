---
id: 60139f2f3a99b79458fe276e
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 匹配字符串的开头和结尾
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

匹配字符串的开头和结尾

回顾一下之前我们学习的知识，正则表达式可以用于查找多项匹配。还可以查询字符串中符合指定匹配模式的字符。

在之前的文章中，我们介绍过在字符集中插入符号（^）来创建一个否定字符集，形如[^icoderoad]。现在我们介绍另外一种用法，在字符集之外，插入符号（^）用于字符串的开头搜寻匹配模式。

let strTest = "路条编程(www.icoderoad.com)欢迎您！";
let testRegex = /^路条编程/;
let result = testRegex.test(strTest);
console.log( result )  ;
// => true

strTest = "您好，路条编程(www.icoderoad.com)欢迎您！";
result = testRegex.test(strTest);
console.log( result )  ;
// => false

由以上代码可知，我们设置了以 路条编程 开头的正则表达式进行模式匹配，通过在一个以 路条编程 开头和另一个不以 路条编程 开头的字符串进行测试，并将结果输出在控制台，第一个测试结果为 true ,第二个测试结果为 false。

上面我们学习了使用 ^ 符号来搜寻字符串开头的匹配模式。还有一种方法可以搜寻字符串结尾的匹配模式。

可以使用美元符号 $ 来搜寻字符串结尾的匹配模式。

let strTest = "路条编程(www.icoderoad.com)欢迎您！";
let testRegex = /欢迎您！$/;
let result = testRegex.test(strTest);
console.log( result )  ;
// => true

strTest = "路条编程不仅是在线学习编程的平台，也是学习编程的友好社区！";
result = testRegex.test(strTest);
console.log( result )  ;
// => false


以上代码我们设置了以 欢迎您！ 结尾的正则表达式进行模式匹配，通过在一个以 欢迎您！ 结尾和另一个不以 欢迎您！ 结尾的字符串进行测试，并将结果输出在控制台，第一个测试结果为 true ,第二个测试结果为 false。


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
