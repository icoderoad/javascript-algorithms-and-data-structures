---
id: 607245895e821511b423e7d9
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 Mixin 在不相关对象之间添加共同行为

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 Mixin 在不相关对象之间添加共同行为

经过我们前面文章中介绍的示例可知，行为是可以通过继承来共享的。然而，在有些情况下，继承不是最好的解决方案。继承不适用于不相关的对象，比如 Bird 和 Airplane 。虽然它们都可以飞行，但是 Bird 并不是一种 Airplane，反之亦然。

对于不相关的对象，更好的方法是使用 mixins。mixin 允许其他对象使用函数集合。

混合（mixin）是一个 class 或者 interface，其中部分或全部 methods 与 properties 未实现，需要另一个 class 或者 interface 来提供这些缺失的实现。

新的类或者接口包括混合所有的以及自有的属性和方法。所有方法和属性的使用方法在混合或混合的实现中保持一致。

混合的优点在于：可用于简化多个接口需要包含相同的方法何与属性的 API 的设计。

下面我们定义一个飞行的方法，示例代码如下所示：

let flyMixin = function(obj) {
  obj.fly = function() {
    console.log("飞行中......");
  }
};

flyMixin 能接受任何对象，并为其提供 fly 方法。

let bird = {
  name: "愤怒的小鸟",
  numLegs: 2
};

let plane = {
  model: "747",
  numPassengers: 2021
};

flyMixin( bird );
flyMixin( plane );

这里的 flyMixin 接收了 bird 和 plane 对象，然后将 fly 方法分配给了每一个对象。现在 bird 和 plane 都可以飞行了。

bird.fly();
 // => 飞行中......

plane.fly(); 
// => 飞行中......


大家需要注意下： mixin 是如何允许相同的 fly 方法被不相关的对象 bird 和 plane 实例重用的。

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
