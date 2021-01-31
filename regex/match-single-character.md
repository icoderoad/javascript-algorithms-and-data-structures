---
id: 600cc07214c4505926fa944f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将单个字符与多种可能性匹配
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

将单个字符与多种可能性匹配

前面文章我们已经介绍了文字匹配模式（/literal/）和通配符（/./）。这是正则表达式的两种极端情况，一种是精确匹配，而另一种则是匹配所有。在这两种极端情况之间有一个平衡选项。
可以使用字符集搜寻具有一定灵活性的文字匹配模式。可以把字符集放在方括号（[和]）之间来定义一组需要匹配的字符串。

例如，如果想要匹配 "bag"、"big" 和 "bug"，但是不想匹配 "bog"。可以创建正则表达式 /b[aiu]g/ 来执行此操作。[aiu] 是只匹配字符"a"、"i"或者"u"的字符集。

let bigStr = "big";
let bagStr = "bag";
let bugStr = "bug";
let bogStr = "bog";
let bgRegex = /b[aiu]g/;
console.log( bigStr.match(bgRegex)) ; 
// => ["big", index: 0, input: "big", groups: undefined] 

console.log(bagStr.match(bgRegex)); 
// => ["bag", index: 0, input: "bag", groups: undefined]

console.log(bugStr.match(bgRegex)); // Returns ["bug"]
// => ["bug", index: 0, input: "bug", groups: undefined]

console.log(bogStr.match(bgRegex)); 
// => null


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
