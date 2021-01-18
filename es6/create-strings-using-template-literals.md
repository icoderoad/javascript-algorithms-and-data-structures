---
id: 5ff80a891291983bb7fa860f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用模板字面量创建字符串
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用模板字面量创建字符串。

模板字符串是 ES6 的另外一项新的功能。这是一种可以轻松构建复杂字符串的方法。

模板字面量 是允许嵌入表达式的字符串字面量。可以使用多行字符串和字符串插值功能。它们在 ES2015 规范的先前版本中被称为“模板字符串”。

语法：

`string text`

`string text line 1
 string text line 2`

`string text ${expression} string text`

tag `string text ${expression} string text`

描述：

模板字符串使用反引号 (` `) 来代替普通字符串中的用双引号和单引号。模板字符串可以包含特定语法（${expression}）的占位符。占位符中的表达式和周围的文本会一起传递给一个默认函数，该函数负责将所有的部分连接起来，如果一个模板字符串由表达式开头，则该字符串被称为带标签的模板字符串，该表达式通常是一个函数，它会在模板字符串处理后被调用，在输出最终结果前，你都可以通过该函数来对模板字符串进行操作处理。在模版字符串内使用反引号（`）时，需要在它前面加转义符（\）。

模板字符串可以使用多行字符串和字符串插值功能。

请看以下代码：

const site = {
  name: "路条编程",
  domain: "www.icoderoad.com"
};

const welcomeMsg = `欢迎访问${site.name}!
请输入网站域名 ${site.domain} 访问网站。`;

console.log(welcomeMsg); 
// => 欢迎访问路条编程!
// => 请输入网站域名 www.icoderoad.com 访问网站。

上面代码中许多需要注意的地方： 首先，上面的例子使用了反引号（`）而不是引号（' 或者 "）定义字符串。 其次，注意字符串是多行的，不管是代码还是输出。这是因为在字符串内插入了 \n。 上面使用的 ${variable} 语法是一个占位符。这样一来，您将不再需要使用 + 运算符来连接字符串。当需要在字符串里增加变量的时候，只需要在变量的外面括上 ${ 和 }，并将其放在字符串里就可以了。 这个新的方式使您可以更灵活的创建复杂的字符串。

下面我们介绍一个完整的示例。使用模板字符串的反引号的语法来展示 result 对象的 failure 数组内的每个条目。每个条目应该括在带有 text-warning 类属性的 li 标签中，并赋值给 resultDisplayArray 。

使用遍历方法（可以是任意形式的循环）输出指定值。

const result = {
  success: ["max-length", "no-amd", "prefer-arrow-functions"],
  failure: ["no-var", "var-on-top", "linebreak"],
  skipped: ["no-extra-semi", "no-dup-keys"]
};

function makeList(arr) {
  "use strict";

  const failureItems = arr.map(item => `<li class="text-warning">${item}</li>`);
  return failureItems;
}
const failuresList = makeList(result.failure);
console.log( failuresList );
// => ["<li class="text-warning">no-var</li>", "<li class="text-warning">var-on-top</li>", "<li class="text-warning">linebreak</li>"]

const skipped = makeList(result.skipped);
console.log( skipped );
// => ["<li class="text-warning">no-extra-semi</li>", "<li class="text-warning">no-dup-keys</li>"]

const success = makeList(result.success);
console.log( success );
// => ["<li class="text-warning">max-length</li>", "<li class="text-warning">no-amd</li>", "<li class="text-warning">prefer-arrow-functions</li>"]

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
