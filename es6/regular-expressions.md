---
id: 60052ab44736bbd3aba1151e
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 正则表达式简介及测试方法
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

正则表达式简介及测试方法

正则表达式是表示搜索模式的特殊字符串。也被称为 “regex” 或 “regexp”，它们帮助程序员匹配、搜索和替换文本。正则表达式可能显得很神秘，因为一些字符有特殊的含义。目标是将符号和文本组合成一个模式，该模式与您想要的匹配，但只与您想要的匹配。在 JavaScript中，正则表达式也是对象。这些模式被用于 RegExp 的 exec 和 test 方法, 以及 String 的 match、matchAll、replace、search 和 split 方法。本专题将介绍字符、一些快捷方式以及编写正则表达式的常见用法。

在编程语言中，正则表达式用于匹配指定的字符串。通过正则表达式创建匹配模式（规则）可以帮您完成指定匹配。
如果想要在字符串"路条编程欢迎您！"中匹配到"路条"这个单词，可以使用如下正则表达式：/路条/。
注意：正则表达式中不需要引号。
JavaScript 中有多种使用正则表达式的方法。测试正则表达式的一种方法是使用.test()方法。.test()方法会把编写的正则表达式和字符串（即括号内的内容）匹配，如果成功匹配到字符，则返回true，反之，返回false。
let testStr = "路条编程(www.icoderoad.com)欢迎您！";
let testRegex = /icode/;
console.log(testRegex.test(testStr));
// => true

上面的代码使用正则对象的.test()方法，检测字符串testStr 中是否符包含 icode 字符串，将测试后的结果输出在控制台，控制台输出结果为 true。

今天就讲到这里，如果有问题需要咨询，大家可以直接留言或扫下方二维码关注公众号。也可以添加 happyzjp 微信受邀加入学习社群，我们会尽力为你解答。

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
