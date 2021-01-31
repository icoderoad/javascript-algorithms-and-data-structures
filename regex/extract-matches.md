---
id: 600a53be91b0e1d06a048e85
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过 .match() 方法提取匹配项
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

通过 .match() 方法提取匹配项

到目前为止，我们介绍过的知识中，只是检查了一个匹配模式是否存在于字符串中。还可以使用 .match() 
方法来提取找到的实际匹配项。.match() 方法是一个在字符串中执行查找匹配的 String 方法，它返回一个数组，在未匹配到时会返回 null。

可以使用字符串来调用 .match() 方法，并在括号内传入正则表达式。以下是一个示例：

let ourStr = "您好, 编程小白。路条编程(www.iCodeRoad.com)欢迎您！";
let result = ourStr.match(/iCodeRoad/);
console.log( result );
// => ["iCodeRoad", index: 18, input: "您好, 编程小白。路条编程(www.iCodeRoad.com)欢迎您！", groups: undefined]

result = ourStr.match(/hello/);
console.log( result );
// => null

ourStr = "正则表达式";
let ourRegex = /表达式/;
result = ourStr.match(ourRegex);
console.log( result );

// => ["表达式", index: 2, input: "正则表达式", groups: undefined]

通过以上代码可以看出，通过 match() 提取单词 iCodeRoad 和 hello ，分别返回相应数组和 null 。说明 .match() 方法执行查找匹配时返回数组，不匹配时返回 null。

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
