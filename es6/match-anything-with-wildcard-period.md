---
id: 600cb20814c4505926fa944e
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 用通配符 . 匹配任何内容
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

用通配符 . 匹配任何内容

有时不知道或不需要匹配模式中的确切字符。如果要精确匹配到完整的单词，那出现一个拼写错误就会匹配不到。幸运的是，JavaScript 语言中可以使用通配符 . 来处理这种情况。

通配符.
（小数点）默认匹配除换行符之外的任何单个字符。可以像使用正则表达式中任何其他字符一样使用通配符。例如，如果想匹配 "hug"、"huh"、"hut" 和 "hum"，可以使用正则表达式 /hu./ 匹配以上四个单词。

let humStr = "I'll hum a song";
let hugStr = "Bear hug";
let huRegex = /hu./;
console.log( huRegex.test(humStr) );
// => true

console.log( huRegex.test(hugStr)); 
// => true

下面我们做个完整的练习，使用正则表达式 tRegex 以匹配字符 "run"、"sun"、"fun"、"pun"、"nun" 和 "bun"。如果要实现相应的匹配规则，正则表达式应该使用通配符 . 来实现。示例代码如下所示：

let testStr = "Let's have fun with regular expressions!";
let tRegex = /.un/; 
let result = tRegex.test( testStr );
console.log( result );
// => true

testStr = "Let us go on a run.";
result = tRegex.test( testStr );
console.log( result );
// => true

testStr ='The sun is out today.';
result = tRegex.test( testStr );
console.log( result );
// => true

testStr ='Coding is a lot of fun.';
result = tRegex.test( testStr );
console.log( result );
// => true

testStr ='Seven days without a pun makes one weak.';
result = tRegex.test( testStr );
console.log( result );
// => true

testStr ='One takes a vow to be a nun.';
result = tRegex.test( testStr );
console.log( result );
// => true

testStr ='She got fired from the hot dog stand for putting her hair in a bun.';
result = tRegex.test( testStr );
console.log( result );
// => true

testStr ='我们在项目的代码审查过程中，发现了代码中的一些 bug .';
result = tRegex.test( testStr );
console.log( result );
// => false

以上代码进行了相应规则的匹配测试，只有最后一个测试返回 false , 其中其他测试字符串中包含 un 的单词在控制台都返回 true 。由此可知，通过用通配符 . 可以匹配任何单一内容。

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
