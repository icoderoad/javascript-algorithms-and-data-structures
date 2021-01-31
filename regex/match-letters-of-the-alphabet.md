---
id: 600f9b8551fd4a8fb7cf8ab0
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 匹配字母表中的字母
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

匹配字母表中的字母

前端文章我们介绍了如何使用字符集来指定要匹配的一组字符串，但是当需要匹配大量字符（例如，字母表中的每个字母）时，有一种写法可以让实现这个功能变得更简单。

在字符集中，可以使用连字符（-）来定义要匹配的字符范围。

例如，要匹配小写字母 a 到 e，可以使用语句 [a-e] 进行匹配。

let catStr = "cat";
let batStr = "bat";
let matStr = "mat";
let bgRegex = /[a-e]at/;
let result = catStr.match(bgRegex); 
console.log( result );
// => ["cat", index: 0, input: "cat", groups: undefined]

result = batStr.match(bgRegex); 
console.log( result );
// => ["bat", index: 0, input: "bat", groups: undefined]

result = matStr.match(bgRegex); 
console.log( result );
// => null

以上代码通过 连字符（-）定义 a - e 的字符，可以匹配 a - e 开头的 + at 的单词，控制台输出结果如上 // =>  后面内容所示。 m 开头的单词超出了连字符的字符范围，所以匹配结果为 null 。

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
