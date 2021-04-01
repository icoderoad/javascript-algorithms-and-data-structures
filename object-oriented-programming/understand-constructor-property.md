---
id: 6065176b3b679f7f45366aeb
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 对象构造函数属性简介
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

对象构造函数属性简介

今天我们先创建狗和猫两个动物对象，具体对象定义如下所示：
function Dog(name) {
  this.name = name;
  this.numLegs = 4;
}

function Cat(name) {
  this.name = name;
  this.numLegs = 4;
}

然后创建的实例对象 dog 和 tom 都有一个特殊的 constructor 属性，constructor 是一种用于创建和初始化 class 创建的对象的特殊方法。

在一个类中只能有一个名为 “constructor” 的特殊方法。 一个类中出现多次构造函数 (constructor)方法将会抛出一个 SyntaxError 错误。

在一个构造方法中可以使用 super 关键字来调用一个父类的构造方法。

如果没有显式指定构造方法，则会添加默认的 constructor 方法。

如果不指定一个构造函数(constructor)方法, 则使用一个默认的构造函数(constructor)。

let dog = new Dog("欢欢");
let cat = new Cat("乐乐");

console.log(dog.constructor === Dog); 
// => true

console.log(cat.constructor === Cat);  
// => true

大家需要注意到的是这个 constructor 属性是对创建这个实例的构造函数的一个引用。 constructor 属性存在的一个优势是，我们可以通过检查这个属性来找出它是一个什么样的对象。

下面是一个例子，来看看是怎么使用的：

function checkDog(animal) {
  if (animal.constructor === Dog) {
    return true;
  } else {
    return false;
  }
}

console.log( checkDog(dog) );
// => true


console.log( checkDog(cat) );
// => false

注意：由于 constructor 属性可以被重写, 后面的文章中会介绍，所以使用 instanceof 方法来检查对象的类型会更好。

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
