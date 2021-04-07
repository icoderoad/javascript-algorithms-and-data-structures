---
id: 606bfa634f4680b48da18413
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用继承避免重复的代码开发
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用继承避免重复的代码开发

在代码开发过程中，有一条原则叫做：Don't Repeat Yourself，常以缩写形式DRY出现，意思是“不要重复开发代码”。编写重复代码会产生的问题是：任何改变都需要去多个地方修复所有重复的代码。这通常意味着我们需要做更多的工作，会产生更高的出错率。

请观察下面的示例，Cat 和 Dog 共享 describe 方法：

Cat.prototype = {
  constructor: Cat,
  describe: function() {
    console.log("我的宠物的名称为 " + this.name);
  }
};

Dog.prototype = {
  constructor: Dog,
  describe: function() {
    console.log("我的宠物的名称为 " + this.name);
  }
};

我们可以看到 describe 方法在两个地方重复定义了。根据以上所说的 DRY 原则，我们可以通过创建一个动物的 Animal 超类（或者父类）来重写这段代码：

function Cat(name) {
  this.name = name;
}

function Dog(name) {
  this.name = name;
}

function Animal() { };

Animal.prototype = {
  constructor: Animal, 
  describe: function() {
    console.log("我的宠物的名称为 " + this.name);
  }
};

Animal 构造函数中定义了 describe 方法，我们将 Cat 和 Dog 这两个构造函数的方法删除掉，改为继承基类 Animal 的方式，调整代码如下所示：

Cat.prototype = {
  constructor: Cat
};

Dog.prototype = {
  constructor: Dog
};

Cat.prototype = new Animal();
Dog.prototype = new Animal();

let cat = new Cat("飞天");
let dog = new Dog("黑豆");
 
console.log( cat.describe() );
// => 我的宠物的名称为 飞天 

console.log( dog.describe() );
// => 我的宠物的名称为 黑豆

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
