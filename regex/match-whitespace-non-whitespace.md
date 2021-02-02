---
id: 6018e3f206eb68bef4110398
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 匹配空白字符和非空白字符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

匹配空白字符和非空白字符

到目前为止，前面的文章中我们学习了通过正则表达式匹配字母和数字。我们通过正则表达式还可以匹配字母之间的空格。

可以使用 \s 搜寻空格，其中 s 是小写。此匹配模式不仅匹配空格，还匹配回车符、制表符、换页符和换行符，可以将其视为与 [\r\t\f\n\v] 匹配功能类似。下面我们以流利说.英语中一段和程序员相关的英语作为示例，代码如下所示：

let engStr = "I code and decode computer programs. I`m a programmer." // 我编码和解码电脑程序，我是个程序员。
let spaceRegex = /\s/g;
let result = engStr.match(spaceRegex);
console.log( result.length );
// => 8

上面代码我们给变量 engStr 赋值一个程序员相关的英语，变量 spaceRegex 设置为 /\s/g ，在全局范围内搜寻空格。通过 match 方法进行正则匹配，将结果赋值给变量 result , 将结果在控制打印输出，控制台输出结果为 8。

上面我们已经学会了如何使用带有小写 s 的缩写 \s 来搜寻空白字符，我们还可以搜寻除了空格之外的所有内容。

我们可以使用 \S 搜寻非空白字符，其中 S 是大写。此匹配模式将不匹配空格、回车符、制表符、换页符和换行符。可以认为这类似于元字符 [^\r\t\f\n\v] 实现功能一致。
下面我们继续以程序员相关的英文为例，对英文中非空格字符串进行匹配并计算字符长度，代码示例如下所示：

let engStr = "I code and decode computer programs. I`m a programmer." // 我编码和解码电脑程序，我是个程序员。
let nonSpaceRegex = /\S/g;
let result = engStr.match(nonSpaceRegex); 
console.log( result.length );
// => 46

上面代码将正则表达式进行了调整，给变量 nonSpaceRegex 赋值为 /\S/g，在全局范围内进行非空格字符匹配查找，将结果赋值给变量 result，并将结果输出至控制台，控制台输出结果为 46。

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
