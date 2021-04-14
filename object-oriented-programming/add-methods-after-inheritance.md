---
id: 6071535442bd623396594dc8
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 从父类继承后在子类中添加方法

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

从父类继承后在子类中添加方法

从父类继承其原型对象的构造函数除了继承的方法之外，还可以有添加自己的方法。

下面我们继续以 Cat 与 Animal 的继承关系为示例，Cat 是一个构造函数，它继承了 Animal 构造函数的原型, 具体示例代码如下所示：

function Animal() { }

Animal.prototype.run = function() {
  console.log("小步快跑中....^_^");
};

function Cat() { }

Cat.prototype = Object.create(Animal.prototype);

Cat.prototype.constructor = Cat;

除了从 Animal 构造函数继承的行为之外，还需要给 Cat 对象添加它独有的行为。这里，我们给 Cat 对象添加一个 eat()

方法。方法会以一种与其他构造函数相同的方式添加到 Cat 的原型中：

Cat.prototype.eat = function() {
  console.log("喵星人，开饭啦!");
};

现在 Cat 的实例中就有了 run() 和 eat() 这两个方法：

let cat = new Cat();

console.log( cat.run() ); 
// => 小步快跑中....^_^

console.log( cat.eat() ); 
// => 喵星人，开饭啦!


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
