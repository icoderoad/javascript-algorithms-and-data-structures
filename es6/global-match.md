---
id: 600a53be91b0e1d06a048e85
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过模式进行全局匹配
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

通过模式进行全局匹配

到目前为止，我们文章中介绍的知识能提取或搜寻一次模式匹配。类似下面的代码示例

let testStr = "路条编程, 路条编程, 路条编程";
let ourRegex = /路条编程/;
let result = testStr.match(ourRegex);
console.log( result );
// => ["路条编程", index: 0, input: "路条编程, 路条编程, 路条编程", groups: undefined]

若要多次搜寻或提取模式匹配，可以使用可选参数 g 。

let testStr = "路条编程, 路条编程, 路条编程";
let repeatRegex = /路条编程/g;
result = testStr.match(repeatRegex);
console.log( result );
// =>["路条编程", "路条编程", "路条编程"]


注意：在正则表达式上可以有多个可选参数，比如 /iCodeRoad/gi。例如下面的代码:

let siteStr = "您好, 编程小白。路条编程(www.iCodeRoad.com)欢迎您！";
let siteRegex = /icoderoad/gi; 
let result = siteStr.match(siteRegex);;
console.log( result );
// => ["iCodeRoad"]

以上代码搜索站点字符串中的 icoderoad 字符串，使用全局参数 g 和 忽略大小写标志 i 进行字符串匹配，匹配结果包含一个元素 ["iCodeRoad"]。

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
