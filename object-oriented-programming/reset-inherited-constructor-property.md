---
id: 606fffd234df632701259faa
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 重置对象继承的构造函数属性

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

重置对象继承的构造函数属性

当一个对象从另一个对象那里继承了其原型，那它也继承了父类的 constructor 属性。

请看下面的示例：

function Animal() { }

function Cat() { }

Cat.prototype = Object.create(Animal.prototype);

let cat = new Cat();

console.log( cat.constructor );
// => ƒ Animal() { }

但是 cat 和其他所有 Cat 的实例都应该表明它们是由 Cat 创建的，而不是由 Animal 创建的。为此，咱们可以手动把 Cat 的 constructor 属性设置为 Cat 对象，示例代码如下所示：

Cat.prototype.constructor = Cat;

console.log( cat.constructor );
// => ƒ Cat() { }


下面我们做个完整的练习，返回 Cat 和 Dog 对象各自的构造函数的一个示例，具体代码如下所示：

function Animal() { }

function Cat() { }

function Dog() { }

Cat.prototype = Object.create(Animal.prototype);

Dog.prototype = Object.create(Animal.prototype);

Cat.prototype.constructor=Cat;

Dog.prototype.constructor=Dog;

let cat = new Cat();

let dog = new Dog();

console.log( cat.constructor );
// => ƒ Cat() { }

console.log( dog.constructor );
// => ƒ Dog() { }

根据以上代码的输出结果可知， Cat 对象和 Dog 对象的构造函数返回的不是 Animal，而是各自对象的构造函数。

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
