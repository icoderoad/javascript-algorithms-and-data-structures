---
id: 606eb219afd463e55c47d23d
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将子类的原型设置为父类实例

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

将子类的原型设置为父类实例

在上篇文章中，我们学习了从超类（或者叫父类） Animal 继承其行为的第一个步骤：创建一个 Animal 的实例。

本文我们将学习第二个步骤：给子对象（或者子类）设置原型。这样一来，Cat 就是 Animal 的一个实例了。

Cat.prototype = Object.create(Animal.prototype);

请记住，原型类似于创建对象的“配方”。从某种意义上来说，Cat 对象的配方包含了 Animal 构造函数的所有关键“成分”。

完整代码如下所示：

function Animal() { }

Animal.prototype = {
  constructor: Animal,
  run: function() {
    console.log("小步快跑中....^_^");
  }
};

function Cat() { }

Cat.prototype = Object.create(Animal.prototype);

let cat = new Cat("汤姆");
console.log(cat.run());
// => 小步快跑中....^_^


cat 继承了 Animal 构造函数的所有属性，其中包括了 run 方法。



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
