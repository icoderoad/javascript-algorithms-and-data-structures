---
id: 60077af355e14a557db01f3f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 同时用多种模式匹配文字字符串
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

同时用多种模式匹配文字字符串

前面文章中，我们介绍了使用正则表达式/icoderoad/，可以在其他字符串中查找 "icoderoad" 字符串。

这对于搜寻单个字符串非常有用，但仅限于一种匹配模式。您也可以使用 | 操作符来匹配多个规则来查找多个字符串。

此操作符匹配操作符前面或后面的字符。例如，如果您想匹配 "路条" 或 "编程"，您需要的正则表达式是 /路条|编程/。

您还可以匹配多个规则，这可以通过添加更多的匹配模式来实现。这些匹配模式将包含更多的 | 操作符来分隔它们，比如/路条|编程|icoderoad/。

下面我们来做个练习，以流利说.英语中夏日水果中的一句英语为例，具体代码如下所示：

let engString = "Yep, I love cherries in season, they are yummy.";
let engRegex = /cherries|watermelon|coconuts/; 
let result = engRegex.test(engString);
 
 上面正则表达式 engRegex 会匹配 "cherries"、"watermelon" 或者 "coconuts"。

我们可以将 engString 换成对应的 "watermelon" 或者 "coconuts" ，看下对应的测试结果，具体完整代码如下所示：

let engString = "Yep, I love cherries in season, they are yummy.";
let engRegex = /cherries|watermelon|coconuts/; 
let result = engRegex.test(engString);
console.log( result );
// => true

engString = "Yep, I love watermelon in season, they are yummy.";
result = engRegex.test(engString);
console.log( result );
// => true

engString = "Yep, I love coconuts in season, they are yummy.";
result = engRegex.test(engString);
console.log( result );
// => true

在控制台执行以上代码后，我们会在控制台看到三行的输出结果都为 true,说明此正则表达式，可以同时用多种模式匹配文字字符串。

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
