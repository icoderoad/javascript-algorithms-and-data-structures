---
id: 601d0a9fe491e4cecc80d653
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 检查混合字符组和删除开头和结尾的空白
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

检查混合字符组和删除开头和结尾的空白

有时候我们想使用正则表达式里的括号 () 来检查字符组。

如果想在字符串找到 icoderoad 或 icodelife，可以这个正则表达式：/icode(road|life)/g。

然后使用 test() 方法检查 test 字符串里面是否包含字符组。

let testStr = "icoderoad";
let testRegex = /icode(road|life)/g;
let result = testRegex.test(testStr);
console.log( result );
// => true

有时字符串周围存在的空白字符并不是必需的。字符串的典型处理是删除字符串开头和结尾处的空格。

编写一个正则表达式并使用适当的字符串方法删除字符串开头和结尾的空格。

注意：字符串的 .trim() 方法可以实现同样的效果，这次我们需要使用正则表达式来完成此练习，代码示例如下所示：

let welcomeMsg = "   路条编程(www.icoderoad.com)欢迎您！  ";
let testRegex = /^\s+|\s+$/g; 
let result = welcomeMsg.replace(testRegex, "");
console.log( result );
// => 路条编程(www.icoderoad.com)欢迎您！

以上代码以通过执行字符串的 replace 方法，调用正则表达式 testRegex，替换成 "" ,并将结果赋值给 result ,将结果输出到控制台，最终控制台输出的结果为 “路条编程(www.icoderoad.com)欢迎您！”，最终结果不包含了开头和结尾的空白。



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
