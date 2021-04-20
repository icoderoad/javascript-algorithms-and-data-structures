---
id: 6077d0d65ae924170ccdc571
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 函数式编程原则及介绍

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

函数式编程原则及介绍

函数式编程是一种基于函数评估的软件开发方法。像数学一样，编程中的函数把输入映射到输出，从而产生一个结果。您可以通过多种方式组合基本函数来构建越来越复杂的程序。

函数式编程遵循以下几个核心原则：

函数独立于程序状态或全局变量。他们只依赖传入他们的参数来进行计算；

函数试图限制对程序状态的任何更改，并避免对保存数据的全局对象进行更改；

函数在程序中的副作用最小；

函数式编程软件开发方法将程序分解为小的、可测试的部分；

函数式编程是一种方案简单、功能独立、对作用域外没有任何副作用的编程范式。

INPUT -> PROCESS -> OUTPUT

函数式编程：

1）功能独立——不依赖于程序的状态（比如可能发生变化的全局变量）；

2）纯函数——同一个输入永远能得到同一个输出；

3）有限的副作用——可以严格地限制函数外部对状态的更改。

下面我们介绍一个完整的例子，我朋友是卖奶茶的，我准备使用程序为他定制一个奶茶外卖小程序，使用函数式编程方法，按订单数量，返回预订的奶茶订单。
具体代码实现如下所示：

const milkTea = () => "milkTea";

const getTea = numOfCups => {
  const teaCups = [];

  for (let cups = 1; cups <= numOfCups; cups ++) {
    const teaCup = milkTea();
    teaCups.push(teaCup);
  }

  return teaCups;
};

const milkTeaOrders = getTea(6); 

console.log(milkTeaOrders);

// => ["milkTea", "milkTea", "milkTea", "milkTea", "milkTea", "milkTea


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
