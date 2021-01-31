---
id: 6015023621776672a004cbb7
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 匹配所有的字母和数字和非字母和数字
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

匹配所有的字母和数字和非字母和数字

前面的文章中，我们已经介绍过使用元字符，可以使用[a-z]搜寻字母表中的所有字母。这种元字符是很常见的，它有一个缩写，但这个缩写也包含额外的字符。

JavaScript 语言中与字母表匹配的最接近的元字符是 \w ，这个缩写等同于[A-Za-z0-9_]。它不仅可以匹配大小写字母和数字，而且还会匹配下划线字符（_）。

let testRegex = /[A-Za-z0-9_]+/;
let testRegex2 = /\w+/;
let numbers = "1088";
let siteName = "icoderoad";
let result = testRegex.test(numbers); 
console.log( result );
// => true

result = testRegex2.test(numbers); 
console.log( result );
// => true

result = testRegex.test(siteName); 
console.log( result );
// => true

result = testRegex2.test(siteName); 
console.log( result );
// => true

以上代码，通过两个不同的正则表达式，进行匹配测试，一个是长的元字符正则，一个是简写的表达式，两个正则测试两个不同的字符串并将结果输出至控制台，控制台输出结果都为 true。 经过以上测试可得，两个正则表达式的效果相同。

经过上面的介绍，我们已经了解了可以使用缩写 \w 来匹配字母和数字 [A-Za-z0-9_] 。不过，有时我们想要搜寻的匹配模式是非字母数字字符。我们应该如何实现呢？
我们可以使用 \W 搜寻和 \w 相反的匹配模式。

注意：相反匹配模式使用大写字母，此缩写与 [^A-Za-z0-9_] 效果是一样的。

下面我们来做个练习，代码如下所示：

let shortRegex = /\W/;
let numbers = "42%";
let welcomeMsg = "welcoming!";
let result2 = numbers.match(shortRegex); 
console.log( result2 );
// => ["%", index: 2, input: "42%", groups: undefined]

result2 = welcomeMsg.match(shortRegex); 
console.log( result2 );
// => ["!", index: 9, input: "welcoming!", groups: undefined]

经过以上代码测试，通过使用简写 \W 正则匹配与 [^A-Za-z0-9_] 效果是一样的。



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
