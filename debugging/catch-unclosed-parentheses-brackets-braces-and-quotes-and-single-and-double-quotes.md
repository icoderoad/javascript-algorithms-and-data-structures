---
id: 602396578b942dd3b47b966e
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 捕获未闭合的括号、方括号、大括号和引号、单引号和双引号的混合用法
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

捕获未闭合的括号、方括号、大括号和引号、单引号和双引号的混合用法

我们在编程过程中，要注意的另一个语法错误是所有的小括号、方括号、花括号、单引号和双引号都必须配对出现。当您编辑代码并插入新代码，新插入的代码带有括号时，很容易忘记括号闭合。此外，在将代码块嵌套到其他代码块时要小心，例如将回调函数作为参数添加到方法中。

避免这种错误的一种方法是，一次性输入完这些符号，然后将光标移回它们之间继续编写。好在，现在大部分编辑器都会帮自动补全。

下面我们给个中括号和小括号的示例，代码如下所示：

let numArr = [28, 32, 63;
let sumArr = numArr.reduce((previous, current =>  previous + current);
console.log(`数组中所有数字之和为: ${ sumArr }`);

我们在浏览器控制台执行以上代码，控制台输出以下错误
unknown: Unexpected token, expected ","  VM73:1 

该错误表示第1行有错误，可以看出缺少结束的中括号，我们给第1行代码增加中括号，调整后代码及控制台输出结果如下：

let numArr = [28, 32, 63];
let sumArr = numArr.reduce((previous, current =>  previous + current);
console.log(`数组中所有数字之和为: ${ sumArr }`);

控制台输出结果：

Uncaught SyntaxError: missing ) after argument list  VM78:2 

上面错误提示第2行缺少结束 ), 我们调整代码并在控制台输出：

let numArr = [28, 32, 63];
let sumArr = numArr.reduce((previous, current) =>  previous + current);
console.log(`数组中所有数字之和为: ${ sumArr }`);

控制台输出结果：
数组中所有数字之和为: 123

经过以上步骤操作，我们完成了基本程序的错误查错，改错的过程。对于初学者来说，程序入门容易，遇到问题排查问题是很麻烦的事情，调试改错需要逐步积累经验，需要一段时间定位问题。看到的错误多了，就可以很快的定位出问题。

在JavaScript 语言中，允许使用单引号 ('') 和双引号 ("") 声明字符串。决定使用哪一个通常看个人偏好，但有一些例外情况需要大家注意。

如果字符串中有缩写或存在一段带引号的文本，您就会明白为什么 JavaScript 语言允许两种引号了。

注意：不要提前用引号结束字符串，这会导致语法错误。

下面是混合使用单引号和双引号的一些示例：


const grouchoContraction = "I've had a perfectly wonderful evening, but this wasn't it.";
const quoteInString = "Groucho Marx once said 'Quote me as saying I was mis-quoted.'";
const uhOhGroucho = 'I've had a perfectly wonderful evening, but this wasn't it.';

当然，在给变量赋值字符串时，只使用一种引号是可以的。您可以使用反斜杠 (\) 转义字符来转义字符串中的引号，下面是带有转义字符的示例：

const allSameQuotes = 'I\'ve had a perfectly wonderful evening, but this wasn\'t it.';

下面我们给出一个双引号完整练习：

let innerHtml = "<p>点击<a href="http://www.icoderoad.com">路条编程</a>访问网站，进行编程练习。</p>";
console.log(innerHtml);

在控制台执行以上代码，会提示 Uncaught SyntaxError: Unexpected identifier ，说明字符串中包含了" ,需要进行转义，调整后代码如下：

let innerHtml = "<p>点击<a href=\"http://www.icoderoad.com\">路条编程</a>访问网站，进行编程练习。</p>";
console.log(innerHtml);
// => <p>点击<a href="http://www.icoderoad.com">路条编程</a>访问网站，进行编程练习。</p>

也可以不使用转义符号，直接在又引号中使用单引号 ‘， 调整后代码如下所示：

let innerHtml = "<p>点击<a href='http://www.icoderoad.com'>路条编程</a>访问网站，进行编程练习。</p>";
console.log(innerHtml);
// => <p>点击<a href='http://www.icoderoad.com'>路条编程</a>访问网站，进行编程练习。</p>

经过上面两种方式调整，代码都可以正常执行。

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
