---
id: 6025bf42df9ec89eefe7d260
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 捕获使用赋值运算符而不是相等运算符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

捕获使用赋值运算符而不是相等运算符

今天是大年初一头一天，路条编程给您拜个年！
祝您度过乐乐呵呵开心年，平平安安吉祥年，团团圆圆幸福年，红红火火好运年，健健康康如意年，财源滚滚发财年。祝关注路条编程的朋友新春快乐，牛年大吉！

今天我们继续介绍调试相关的知识。

捕获使用赋值运算符而不是相等运算符


分支程序，即在满足某些条件时执行不同操作的程序，依赖于 JavaScript 语言中的 if，else if、else 语句。条件有时采取测试一个结果是否等于一个值的形式。

这种逻辑可以表述为“如果 x 等于 y ，则......”，听起来像是可以使用=（即赋值运算符）。然而，这会导致程序中流程出问题。

如前面的文章所述，JavaScript 语言中的赋值运算符 (=) 是用来为变量名赋值的。并且 == 和 === 运算符检查相等性（三等号 === 是用来测试是否严格相等的，严格相等的意思是值和类型都必须相同）。

下面的代码将 x 赋值为 2，表达式 x = y 会在执行后得到 true。JavaScript 语言会把大部分的值都视为 true，除了所谓的 "falsy" 值，即：false、0、""（空字符串）、NaN、undefined 和 null。

下面我们做个完整的练习，代码如下所示：

let x = 7;
let y = 9;
let result = "to come";

if(x = y) {
  result = "Equal!";
} else {
  result = "Not equal!";
}

console.log(result);
// => Equal!


我们在控制台执行以上语言，控制台会输出  Equal! 字符串。实际上输出结果不是我们想要的，大家可以仔细查看下 if 语句， 其中的条件判断应该是使用 == 或 === 来测试是否相等，而不是使用赋值语句 = 来进行条件判断，调整后的代码如下：

let x = 7;
let y = 9;
let result = "to come";

if(x === y) {
  result = "Equal!";
} else {
  result = "Not equal!";
}

console.log(result);
// => Not equal!

在控制台执行以上代码，由于 x 和 y 的值分别是 7和 9，数值不等，所以会执行 else 语句，会将 result 变量赋值为 Not equal!，所以控制台会输出 “Not equal!”。



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
