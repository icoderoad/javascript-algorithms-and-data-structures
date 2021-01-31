---
id: 6010fb952a6e0826e95bf019
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 匹配未指定或出现零次或出现多次的字符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

匹配未指定或出现零次或出现多次的字符

到目前为止，我们已经介绍了一个想要匹配的字符集合，但是也可以创建一个不想匹配的字符集合。这些类型的字符集称为否定字符集。

要创建否定字符集，需要在开始括号后面和不想匹配的字符前面放置插入字符（即^）。

例如，/[^icoderoad]/gi 匹配所有非 icoderoad 字符。注意，字符 .、!、[、@、/ 和空白字符等也会被匹配，该否定字符集仅排除 icoderoad 之中的字符。

有的时候，需要匹配出现一次或者连续多次的的字符（或字符组）。这意味着它至少出现一次，并且可能重复出现。

我们可以通过使用 + 符号来检查情况是否如此。记住，字符或匹配模式必须一个接一个地连续出现。

例如，/i+/g 会在 "icoderoad" 中匹配到一个匹配项，并且返回["i"]。因为 + 的存在，它也会在 "iicoderoad" 中匹配到一个匹配项，然后返回 ["ii"]。

如果它是检查字符串 "icodeicode"，它将匹配到两个匹配项并且返回["i", "i"]，因为 i 字符不连续，在它们之间有一个 code 单词隔开。最后，因为在字符串 "road" 中没有 "i"，因此找不到匹配项。

除了 + 符号以外，还有一个选项可以匹配出现零次或多次的字符。执行该操作的字符叫做星号，即 * 。

下面我们练习一个完整的示例，代码如下所示：

let googleWord = "goooooooogle!";
let gPhrase = "good good study ,day day up"; // 好好学习 天天向上
let oPhrase = "oh my god";
let goPlusRegex = /go+/;
let goStarRegex = /goo*/;
let result = googleWord.match(goPlusRegex);
console.log( result ); // => ["goooooooo", index: 0, input: "goooooooogle!", groups: undefined]

result = googleWord.match(goStarRegex);
console.log( result ); // => ["goooooooo", index: 0, input: "goooooooogle!", groups: undefined]

result = gPhrase.match(goPlusRegex); 
console.log( result ); // => ["goo", index: 0, input: "good good study ,day day up", groups: undefined]

result = oPhrase.match(goPlusRegex); 
console.log( result ); // => ["go", index: 6, input: "oh my god", groups: undefined]

以上代码我们使用 + 和 * 做了相应的匹配测试，通过控制台的输出结果可以看出，正则表达式 goPlusRegex 使用 + 符号来匹配一个或多个符合条件的字符，正则表达式 goStarRegex 使用 * 符号匹配出现的零个或多个 符合条件的 'o' 字符。

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
