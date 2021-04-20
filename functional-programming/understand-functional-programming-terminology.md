---
id: 607a10d8be676dda47bf6782
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 了解函数式编程术语

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

了解函数式编程术语

随着需求讨论的深入，我朋友销售的奶茶，现在想要增加两个新品奶茶：红西柚（Red grapefruit）和木瓜（papaya）。根据朋友新的需求，我们需要重构上篇文章中的 getTea 函数来处理多种奶茶的请求。我们可以修改 getTea 接受一个函数作为参数，使它能够修改奶茶的类型。这让 getTea 更灵活，也使需求变更时为程序员提供更多控制权。

首先，我们将介绍一些术语：

Callbacks 是被传递到另一个函数中调用的函数。您应该已经在其他函数中看过这个写法，例如在 filter 中，回调函数告诉 JavaScript 以什么规则过滤数组。

函数就像其他正常值一样，可以赋值给变量、传递给另一个函数，或从其它函数返回，这种函数叫做头等函数。在 JavaScript 中，所有函数都是头等函数。

一个返回另外一个函数的函数被称为高阶函数

当函数传递给另一个函数或从另一个函数返回时，那些传入或返回的函数可以叫做 lambda。

下面我们继续根据实际场景需求进行程序调整优化，具体场景如下所示：

现在学生要团购 18 杯红西柚奶茶和 26 杯木瓜奶茶，分别下单，我们将两单分别存在 teaOrder1 和 teaOrder2  变量中。优化的完整代码如下所示：

const redGrapefruitTea = () => 'redGrapefruit';

const papayaTea = () => 'papayaTea';

const getTea = (saleTea, num) => {
  const teaCups = [];

  for(let cups = 1; cups <= num; cups ++) {
    const teaCup = saleTea();
    teaCups.push(teaCup);
  }

  return teaCups;
};

const teaOrder1 = getTea(redGrapefruitTea,18);
const teaOrder2 = getTea(papayaTea,26);

console.log(
  teaOrder1,
  teaOrder2
);
// => (18) ["redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit", "redGrapefruit"] (26) ["papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea", "papayaTea"]

根据以上代码可知，getTea 函数增加为两个参数的函数，现在它接收一个函数作为第一个参数，杯数作为第二个参数。


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
