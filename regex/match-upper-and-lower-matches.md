---
id: 601a3c79809da9f2352b8bef
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 指定匹配的上限和下限和只设置匹配下限
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

指定匹配的上限和下限和只设置匹配下限

回顾下我们前面所学知识，我们已经学习了使用加号 + 查找一个或多个字符，使用星号 * 查找零个或多个字符。这些匹配模式都很方便，但有时我们需要匹配一定范围的匹配模式。

我们可以使用数量说明符指定匹配模式的上下限。数量说明符与花括号（ { 和 } ）一起使用。可以在花括号之间放两个数字，这两个数字代表匹配模式的上限和下限。

例如，要在字符串"g和gle"中匹配仅出现 2 到 5 次的字母 o，正则表达式应为/go
{2,5}gle/。

let strTest = "google";

let regexTest = /go{2,5}gle/;
let result = regexTest.test(strTest); 
console.log( result );
// => true

strTest= "gogle";
result = regexTest.test(strTest); 
console.log( result );
// =>  false

上面代码我们设置要匹配的字符串为谷歌的英文名称及少了一个字母 o 的英文字符串，正则表达式变量 regexTest 设置为  /go{2,5}gle/， 指定字符串 g 和 gle 之间字母 o 的数最为 2 到 5，下限为 2，上限为 5，然后通过 test 方法进行测试，并将测试结果赋值给变量 result ，然后将结果变量 result 输出到控制台，控制台输出 true 。然后测试字符串 gogle，字符串 g 和 gle 两个字符串之间只有一个字母 o, 不符合正则匹配条件，控制台输出结果为 false。

上面我们介绍了使用带有花括号的数量说明符来指定匹配模式的上下限。但有时候我们在实际工作中只想指定匹配模式的下限而不需要指定上限。我们需要将上面的匹配规则调整下，在第一个数字后面跟一个逗号即可。

我们继续以谷歌英文名为例，要匹配在字符串 g 和 gle 两个字符串之间至少出现 2 次字母 o 的字符串，正则表达式应该是/go{2,}gle/。

let strTest = "google";
let regexTest = /go{2,}gle/;
let gle30 = "g" + "o".repeat(30) + "gle";
let result = regexTest.test(strTest); 
console.log( result );
// => true

result = regexTest.test(gle30); // 
console.log( result );
// => true

以上代码我们对正则表达式进行了调整，设置为只有下限 2，不设上限，也就是说，在字符串 g 和 gle 两个字符串之间最少有两个字母 0 ，超过两个字母 o 的字符串都符合条件。我们通过 repeat 方法产生了在字符串 g 和 gle 两个字符串之间有 30 个字母 o 的字符，将字符串赋值给变量 gle30, 通过正则表达式 regexTest 进行测试，并将测试结果在控制台输出，控制台输出结果为 true。

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
