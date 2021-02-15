---
id: 602b0286882f4ccb7760760b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用有效的终止条件防止无限循环
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/debuging.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

使用有效的终止条件防止无限循环

本专题最后一个话题是可怕的无限循环。当需要程序运行代码块一定次数或满足条件时，循环是很好的工具，但是它们需要终止条件来结束循环。无限循环可能会使浏览器冻结或崩溃，并导致程序执行混乱，没有人想要这样的结果。

在今天的文章中有一个无限循环的例子——它没有终止条件来摆脱 loopy() 内的 while 循环。注意：不要调用这个函数！

function loopy() {
  while(true) {
    console.log("您好，欢迎访问路条编程网站!");
  }
}
loopy()
// => 4768 您好，欢迎访问路条编程网站!

以上代码在浏览器控制台执行后，会无限制的执行，在控制显示 ”您好，欢迎访问路条编程网站! “ 信息，前面的数字一直在增加，表示重复执行的次数。


程序员的工作是确保最终达到终止条件，该条件告诉程序何时跳出循环。有一种错误是从终端条件向错误方向递增或递减计数器变量。另一种是在循环代码中意外重置计数器或索引变量，而不是递增或递减它。

testFunc() 函数包含一个无限循环，因为终止条件i != 4永远不会为 false (并中断循环) -i 将每次递增 2，然后跳过 4，因为 i 是从奇数开始递增。在终端条件中输入比较运算符，使循环仅在 i 小于或等于 4 的情况下运行。

function testFunc() {
  for (let i = 1; i != 4; i += 2) {
    console.log("程序执行中，当前 i 为 " + i + "!");
  }
}
testFunc() 
// => 程序执行中，当前 i 为 937!

注意：以上程序在控制台谨慎执行，控制台会一直输出当前变量的值，会使浏览器崩溃。



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
