---
id: 601b8ea510a1b7ee6ca066de
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用问号?检查元素和先行断言用法
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

使用问号?检查元素和先行断言用法

我们在实际项目中，有时需要搜寻的匹配模式可能有不确定是否存在的部分。在这种情况时，我们想检查它们，应该使用什么方式进行模式匹配呢？

在 JavaScript 语言中，可以使用问号 ? 指定可能存在的元素。? 将检查前面的零个或一个元素。可以将此符号视为前面的元素是可选的。

以颜色的单词为例，美式英语和英式英语略有不同，可以使用问号来匹配两种拼写。

let american = "color";
let british = "colour";
let testRegex= /colou?r/;
let result = testRegex.test(american); 
console.log( result );
// => true

result = testRegex.test(british); 
console.log( result );
// => true

先行断言是告诉 JavaScript 在字符串中向前查找的匹配模式。当想要在同一个字符串上搜寻多个匹配模式时，这可能非常有用。

有两种先行断言：正向先行断言和负向先行断言。

正向先行断言会查看并确保搜索匹配模式中的存在元素，但实际上并不匹配。正向先行断言的用法是(?=...)，其中...就是需要存在但不会被匹配的部分。

另一方面，负向先行断言会查看并确保搜索匹配模式中的不存在元素。负向先行断言的用法是(?!...)，其中...是希望不存在的匹配模式。如果负向先行断言部分不存在，将返回匹配模式的其余部分。

尽管先行断言有点儿令人困惑，但是下面这些示例会对大家理解这个概念有所帮助。

let quit = "qu";
let noquit = "qt";
let quRegex= /q(?=u)/;
let qRegex = /q(?!u)/;
let result = quit.match(quRegex); 
console.log( result );
// =>  ["q", index: 0, input: "qu", groups: undefined]

result = noquit.match(qRegex); 
console.log( result );
// => ["q", index: 0, input: "qt", groups: undefined]

先行断言的更实际用途是检查一个字符串中的两个或更多匹配模式。这里有一个简单的密码检查器，密码规则是 3 到 6 个字符且至少包含一个数字：

let password = "icode9";
let checkPass = /(?=\w{3,6})(?=\D*\d)/;
let result = checkPass.test(password);
console.log( result );
// => true

上面代码使用了两个正向先行断言，一个用来判断 3 到 6 个字符，另一个用户判断至少包含一个数字，然后对密码变量的值 icode9 进行测试，将结果输出至控制台，控制台输出结果为 true。

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
