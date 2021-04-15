---
id: 6077d0d65ae924170ccdc571
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 立即调用函数表达（IIFE）简介及模块创建

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

立即调用函数表达式（IIFE）简介及模块创建

JavaScript 语言中的一个常见模式就是，函数在声明后立刻执行：

(function () {
  console.log("路条编程欢迎您！");
})(); // 这是一个立即执行的匿名函数表达式

// 在控制台执行后，立即输出 路条编程欢迎您！

注意：函数没有名称，也不存储在变量中。函数表达式末尾的两个括号（）导致它被立即执行或调用。这种模式被叫做立即调用函数表达式或者 IIFE。

IIFE（ 立即调用函数表达式）是一个在定义时就会立即执行的  JavaScript 函数，语法如下所示：

(function () {
    statements
})();

这是一个被称为 自执行匿名函数 的设计模式，主要包含两部分。第一部分是包围在 圆括号运算符 () 

里的一个匿名函数，这个匿名函数拥有独立的词法作用域。这不仅避免了外界访问此 IIFE 中的变量，而且又不会污染全局作用域。

第二部分再一次使用 () 创建了一个立即执行函数表达式，JavaScript 引擎到此将直接执行函数。

一个立即调用函数表达式（IIFE）通常用于将相关功能分组到单个对象或者是模块中。例如，前面文章中定义的一个滑行或飞行的混合类，代码如下所示：

function glideMixin(obj) {
  obj.glide = function() {
    console.log("水上滑行中...");
  };
}

function flyMixin(obj) {
  obj.fly = function() {
    console.log("飞行中...");
  };
}

我们可以将这些 mixins 分成以下模块：

let commonModule = (function () {
  return {
    glideMixin: function(obj) {
      obj.glide = function() {
        console.log("水上滑行中...");
      };
    },
    flyMixin: function(obj) {
      obj.fly = function() {
        console.log("飞行中...");
      };
    }
  }
})(); // 末尾的两个括号导致函数被立即调用

注意：一个立即调用函数表达式（IIFE）返回了一个 commonModule 对象。返回的这个对象包含了作为对象属性的所有 mixin 行为。 

模块模式的优点是，所有的通用行为都可以打包成一个对象，然后由代码的其他部分使用。

下面是一个使用它的完整示例：

let plane = {
  model: "747",
  numPassengers: 2021
};

commonModule.glideMixin( plane );
commonModule.flyMixin( plane );

console.log(plane.glide());
// => 水上滑行中...

console.log(plane.fly());
// => 飞行中...

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
