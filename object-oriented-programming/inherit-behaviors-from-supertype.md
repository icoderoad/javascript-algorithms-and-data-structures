---
id: 606d481bd131b2310ccd9cb1
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 从超类继承对象行为
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

从超类继承对象行为

在上篇文章中，我们创建了一个 Animal 超类，用来定义所有动物共有的行为：

function Animal() { }

Animal.prototype.run = function() {
  console.log("小步快跑中....^_^");
};

在今天的文章中我们将学习如何给 Cat、Dog 重写 Animal 中的方法，而无需重新定义它们。这里我们会用到构造函数的继承特性。 

今天的文章中我们学习第一步：创建一个超类（或者叫父类）的实例。 我们前面已经学会了一种创建 Animal 实例的方法，即使用 new 操作符，代码示例如下所示：

let animal = new Animal();

此语法用于继承时会存在一些缺点，这些缺点对于当前我们现在学习的知识来说太复杂了。现在我们学习另外一种没有这些缺点的方法来替代 new 

操作，在介绍相应的代码前，我们先介绍下 Object.create() 方法的相应用法。

Object.create() 方法创建一个新对象，使用现有的对象来提供新创建的对象的 __proto__。

语法：

Object.create(proto，[propertiesObject])

参数：

proto 新创建对象的原型对象。

propertiesObject 可选。需要传入一个对象，该对象的属性类型参照Object.defineProperties()的第二个参数。如果该参数被指定且不为

undefined，该传入对象的自有可枚举属性(即其自身定义的属性，而不是其原型链上的枚举属性)将为新创建的对象添加指定的属性值和对应的属性描述符。

返回值：

一个新对象，带着指定的原型对象和属性。


代码示例如下所示：

let animal = Object.create(Animal.prototype);

Object.create(obj) 创建了一个新对象，并指定了 obj作为新对象的原型。回忆一下，我们之前说过原型就像是创建对象的“配方”。如果我们把 animal 的原型设置为与 Animal 构造函数的原型一样，那么就相当于让 animal 这个实例的配方与 Animal 其他实例的配方一样了。

console.log( animal.run()); 
// => 小步快跑中....^_^

console.log(animal instanceof Animal);
 // => true

下面我们使用 Object.create 方法给 Animal 创建两个实例：ccat 和 dog, 完整示例代码如下所示：

function Animal() { }

Animal.prototype = {
  constructor: Animal,
  run: function() {
    console.log("小步快跑中....^_^");
  }
};


let cat = Object.create(Animal.prototype); 
console.log( cat.run() );
// => 小步快跑中....^_^

let dog = Object.create(Animal.prototype); 
console.log( dog.run() );
// => 小步快跑中....^_^

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
