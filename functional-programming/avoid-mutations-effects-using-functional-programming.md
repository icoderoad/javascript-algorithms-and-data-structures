---
id: 607d166842d1620a9eb930e5
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用函数式编程避免变化和副作用

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用函数式编程避免变化和副作用

前篇文章中我们介绍的问题出在 tabClose() 函数里的 splice。不幸的是，splice 修改了调用它的原始数组，所以第二次调用它时是基于修改后的数组，才给出了意料之外的结果。

这只是实际工作中的一个小例子，还有更广义的定义——在变量、数组或对象上调用一个函数，这个函数会改变对象中的变量或其他东西。

函数式编程的核心原则之一是不改变任何东西。变化会导致错误。如果一个函数不改变传入的参数、全局变量等数据，那么它造成问题的可能性就会小很多。

前面的例子没有任何复杂的操作，但是 splice 方法改变了原始数组，导致 bug 产生。

我们回想一下，在函数式编程中，改变或变更叫做 mutation，这种改变的结果叫做“副作用”。理想情况下，函数应该是不会产生任何副作用的纯函数。

让我们尝试掌握这个原则：不要改变代码中的任何变量或对象。

我们来练习一个示例，使用 incremNum 函数返回全局变量 gNum 的值增加 1，函数不改变 gNum 的值，incremNum 函数返回的值比 gNum 变量更大的值。的值，incremNum 函数应返回全局 gNum 变量值。具体示例代码如下所示：

var gNum = 4;

function incremNum() {

  return gNum + 1;
}

var tmpNum = incremNum();
console.log(gNum); 
// => 4



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
