---
id: 6006422155e14a557db01f3e
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 匹配文字字符串
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

匹配文字字符串


前面文章中我们介绍了使用正则表达式/icode/搜索到了字符串"icode"。那个正则表达式在字符串中搜寻"icode"的文字匹配。下面是另一个在字符串中搜寻"icoderoad"的示例：

let testStr = "您好, 编程小白。路条编程(www.icoderoad.com)欢迎您！";
let testRegex = /icoderoad/;
let result = testRegex.test(testStr);
console.log( result );
// => true

任何其他形式的 "icoderoad" 都不会被匹配。例如，正则表达式 /icoderoad/ 不会匹配 "Icoderoad" 或者 "ICODEROAD"。

let wrongRegex = /Icoderoad/;
let result2 = wrongRegex.test(testStr);
console.log( result2 );
// => false

后续的文章将为您介绍如何匹配其他形式的字符串。

下面我们再完成一个类似全英文字符串的练习，正则表达式 waldoRegex 只从 waldoIsHiding 字符串中匹配到文本 "Waldo"。

let summerStr = "But the summer sales just started yesterday.";
let salesRegex = /sales/; 
let result = salesRegex.test(summerStr);
console.log(result);
// => true

以上代码执行后，会在控制台输出 result 变量的值为 true。经过多次练习，我们可以得知 test 方法对中文和英文都可以正常匹配并返回结果。

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
