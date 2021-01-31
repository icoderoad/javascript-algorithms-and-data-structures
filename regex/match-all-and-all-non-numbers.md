---
id: 601658fa9f29c4c1298820ce
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 匹配所有数字和所有非数字
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

匹配所有数字和所有非数字

前面文章中我们已经介绍了常见字符串匹配模式的元字符，如字母和数字。另一个比较常见的匹配模式是只寻找数字。现在我们介绍下数字匹配模式。

查找数字字符的缩写是 \d，注意是小写的 d。这等同于元字符 [0-9]，它查找 0 到 9 之间任意数字的单个字符。

下面我们来做个练习，使用缩写 \d 来计算网站版权信息中有多少个数字。

let copyrightStr = "Copyright 2021 ICodeRoad & 路条编程";
let numRegex = /\d/g; 
let result = copyrightStr.match(numRegex).length;
console.log( result );
// => 4

以上代码通过数字正则表达式缩写来匹配数字字符，使用全局状态修正符进行全局范围内进行查找， 将最终查找结果赋值给变量 result ,并将结果在控制台输出，控制台输出结果为 4。

上面我们展示了如何使用带有小写 d 的缩写 \d 的正则表达式来搜寻数字。也可以使用类似的缩写来搜寻非数字，该缩写使用大写的 D。

查找非数字字符的缩写是 \D。这等同于字符串[^0-9]，它查找不是 0 - 9 之间数字的单个字符。

使用非数字缩写 \D 来计算网站版权信息中有多少非数字。

let copyrightStr = "Copyright 2021 ICodeRoad & 路条编程";
let testRegex = /\D/g; 
let result2 = copyrightStr.match( testRegex ).length;
console.log( copyrightStr );
console.log( result2 );
// => 27 

以上代码通过非数字正则表达式缩写来匹配非数字字符，使用全局状态修正符进行全局范围内进行查找， 将最终查找结果赋值给变量 result2 ,并将结果在控制台输出，控制台输出结果为 27。

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
