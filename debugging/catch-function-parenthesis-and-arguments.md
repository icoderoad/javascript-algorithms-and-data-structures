---
id: 60270e6ac389be07b9fdc1e8
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 捕捉函数调用后缺少的括号和错误顺序传递的参数
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/debuging.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

捕捉函数调用后缺少的括号和错误顺序传递的参数

当函数或方法不接受任何参数时，您可能忘记在调用它时加上空的左括号和右括号。通常，函数调用的结果会保存在变量中，供其他代码使用。可以通过将变量值（或其类型）打印到控制台，查看输出究竟是一个函数引用还是函数调用的返回值来检测这类错误。

下面示例中的两个变量是不同的:

function welcomeMsg() {
  return "您好，欢迎访问路条编程网站(www.icoderoad.com)!";
}

let msg1 = welcomeMsg; 
console.log( msg1 );
// => ƒ welcomeMsg() {
//  	return "您好，欢迎访问路条编程网站(www.icoderoad.com)!";
//    }

let msg2 = welcomeMsg(); 
console.log( msg2 );
// => 您好，欢迎访问路条编程网站(www.icoderoad.com)!

以上代码在控制台执行后，变量 1 调用 welcomeMsg 方法无括号， 将一个函数赋值给了变量 1。在控制台输出以 f 为前缀的完整函数。变量 2 调用 welcomeMsg 方法有括号，显示方法返回的字符串。

我们继续讨论调用函数问题，需要注意的下一个 bug 是函数的参数传递顺序错误。 如果参数分别是不同的类型，例如接受数组和整数两个参数的函数，参数顺序传错就可能会引发运行时错误。对于接受相同类型参数的函数，传错参数也会导致逻辑错误或运行结果错误。确保以正确的顺序提供所有必需的参数以避免这些问题。

下面我们做个练习，函数 mathPow 返回基数 (base) 的指数 n 次幂。不幸的是，它没有被正确调用，代码如下所示：

function mathPow(base, n) {
  return Math.pow(base, n);
}

let base = 2;
let n = 5;

// 错误调用
let num = mathPow(n, base);
console.log(num);
// => 25

// 正确调用
num = mathPow( base, n);
console.log(num);
// => 32

以上代码由于参数顺序错误，在控制台执行后，没有逻辑错误。由于调用函数参数顺序不对，本想计算 2 的 5 次幂，结果算成了 5 的 2 次幂。上面代码前半部分为调用参数错误示例，后半部分为正确调用，最终结果在控制台分别输出 25 和 32。

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
