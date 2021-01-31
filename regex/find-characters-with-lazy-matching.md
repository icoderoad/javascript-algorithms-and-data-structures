---
id: 6010fb952a6e0826e95bf019
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 用惰性匹配来查找字符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

用惰性匹配来查找字符

在正则表达式中，贪婪匹配会匹配到符合正则表达式匹配模式的字符串的最长可能部分，并将其作为匹配项返回。另一种方案称为懒惰匹配，它会匹配到满足正则表达式的字符串的最小可能部分。

可以将正则表达式 /i[a-z]*d/ 应用于字符串 "icoderoad"。这个正则表达式是一个以 i 开始，以 d 结束，并且中间有一些字母的匹配模式。

正则表达式默认是贪婪匹配，因此匹配返回为 ["icoderoad"]。它会匹配到适合该匹配模式的最大子字符串。

但是，您可以使用 ? 字符来将其变成懒惰匹配。调整后的正则表达式 /i[a-z]*?d/ 匹配字符串"icoderoad"返回["icod"]。

完整示例如下所示:

let str = "icoderoad";
let regexTest = /i[a-z]*d/;
let tResult = str.match(regexTest);
console.log(tResult);
// => ["icoderoad", index: 0, input: "icoderoad", groups: undefined]

regexTest = /i[a-z]*?d/;
tResult = str.match(regexTest);
console.log(tResult);
// => ["icod", index: 0, input: "icoderoad", groups: undefined]

注意:应该避免使用正则表达式解析 HTML，但是可以用正则表达式匹配 HTML 字符串。

下面我们做个练习，设置正则表达式/<.*?>/，让它返回 HTML 标签 <h2>，而不是文本"<h2>您好，路条编程欢迎您!</h2>"，示例代码如下所示：

let text = "<h2>您好，路条编程欢迎您!</h2>";
let myRegex = /<.*?>/; 
let result = text.match(myRegex);
console.log( result );
// => ["<h2>", index: 0, input: "<h2>您好，路条编程欢迎您!</h2>", groups: undefined]

myRegex = /<.*>/; 
result = text.match(myRegex);
console.log( result );
// => ["<h2>您好，路条编程欢迎您!</h2>", index: 0, input: "<h2>您好，路条编程欢迎您!</h2>", groups: undefined]

在控制台执行以上代码，通过控制台输出结果比较发现，懒惰匹配只匹配出了 <h2>, 贪婪匹配返回了 <h2>您好，路条编程欢迎您!</h2> 。

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
