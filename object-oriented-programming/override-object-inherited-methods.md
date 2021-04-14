---
id: 607245895e821511b423e7d9
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 重写从父类继承的方法

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

重写从父类继承的方法

在上篇文章中，我们学习了一个对象可以通过复制另一个对象的原型来继承其属性或方法：

ChildObject.prototype = Object.create(ParentObject.prototype);

然后，ChildObject 将自己的方法链接到它的原型中：

ChildObject.prototype.methodName = function() {...};

我们还可以重写继承的方法。以同样的方式向 ChildObject.prototype 中添加需要重写的相同名称的方法。 请看下面的举例：Cat 重写了从 Animal 继承来的 eat()方法：

function Animal() { }

Animal.prototype.eat = function() {
  return "小可爱们吃饭了";
};

function Cat() { }

// 继承了 Animal 的所有方法
Cat.prototype = Object.create(Animal.prototype);

// Cat.eat() 重写了 Animal.eat() 方法

Cat.prototype.eat = function() {
  return "喵星人，开饭啦!";
};

下面我们创建一个实例：

let cat = new Cat();

然后调用 cat.eat() 方法，以下为 JavaScript 在 cat 的原型链上寻找方法的过程：

cat => 这里定义了 eat() 方法吗？没有。

Cat => 这里定义了 eat() 方法吗？=> 是的。执行它并停止往上搜索。

Animal => 这里也定义了 eat() 方法，但是 JavaScript 在到达这层原型链之前已停止了搜索。

Object => JavaScript 在到达这层原型链之前也已经停止了搜索。

咱们在控制台打印下 cat 实例 eat() 方法的输出结果，代码如下所示：

console.log( cat.eat() );
// => 喵星人，开饭啦!

通过上面控制台输出结果可知，cat 实例返回的是覆盖后方法返回的结果。

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
