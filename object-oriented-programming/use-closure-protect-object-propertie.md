---
id: 60764dd05c5a4cd218bd45e7
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用闭包保护对象内的属性不被外部修改

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用闭包保护对象内的属性不被外部修改

在前面文章介绍的内容中，cat 有一个公共属性 name。公共属性的定义就是：它可以在 cat 的定义范围之外被访问和更改。

cat.name = "加菲猫";

因此，代码的任何地方都可以轻松地将 cat 的 name 属性更改为任意值。想想密码和银行账户之类的东西，如果代码库的任何部分都可以轻易改变，那么将会引起很多问题。

使属性私有化最简单的方法就是在构造函数中创建变量。可以将该变量范围限定在构造函数中，而不是全局可用。这样，属性只能由构造函数中的方法访问和更改。

在介绍具体示例之前，我们先了解下闭包的概念。一个函数和对其周围状态（lexical environment，词法环境）的引用捆绑在一起（或者说函数被引用包围），这样的组合就是闭包（closure）。

也就是说，闭包让你可以在一个内层函数中访问到其外层函数的作用域。在 JavaScript 中，每当创建一个函数，闭包就会在函数创建的同时被创建出来。

下面代码是一个 Cat 对象的闭包示例：

function Cat() {
  let color = "white"; // 私有变量

  /* cat 对象可用的公共方法 */

  this.getColor = function() { 
    return color;
  };

}

这里的 getColor() 是一种特权方法，因为它可以访问私有属性 color 。这是因为 color 是在与 getColor 相同的上下文中声明的。在 JavaScript 中，函数总是可以访问创建它的上下文。这就叫做闭包。

下面我们给 Cat 对象增加一个 age 年龄属性，在 Cat 对象中声明 age 属性，使其成为私有变量。然后，创建一个返回 age 值的 getAge 方法,调整后的完整代码如下所示：

function Cat() {
  // 私有变量
  let color = "white"; 
  let age = 1;

  /* cat 对象可用的公共方法 */

  this.getColor = function() { 
    return color;
  };

  this.getAge = function() {
  		return age;
  }
}

let cat = new Cat();

console.log( cat.getColor() ); 
// => white

console.log( cat.getAge() ); 
// => 1

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
