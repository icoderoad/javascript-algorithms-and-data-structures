---
id: 60961647ba50c85eb90c93fe
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: JavaScript 中的函数柯里化
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

JavaScript 中的函数柯里化

函数柯里化以 Haskell Brooks Curry 命名，柯里化是指将一个函数分解为一系列函数的过程，每个函数都只接收一个参数。这些函数不会立即求值，而是通过闭包的方式把传入的参数保存起来，直到真正需要的时候才会求值。

换句话说，就是重构函数让它接收一个参数，然后返回接收下一个参数的函数，依此类推。

举个简单的例子：

//非柯里化版
function sum(x, y, z) {
  return x + y + z;
}

sum 函数的柯里化版本的结构不一样。它接收一个参数并返回一个函数。返回的函数中又接收一个参数，返回另一个仍然只接收一个参数的函数...（以此往复）
直到返回的函数接收到最后一个参数时，这个循环才结束。这个最后的函数将会返回数字的总和，如下所示。

//柯里化版
function sum(x) {
  return (y) => {
    return (z) => {
      return x + y + z
    }
  } 
}

console.log(sum(3)(5)(7));
// => 15


柯里化在不能一次为函数提供所有参数情况下很有用。因为它可以将每个函数的调用保存到一个变量中，该变量将保存返回的函数引用，该引用在下一个参数可用时接受该参数。下面是使用柯里化函数的例子：

var sumy = sum(5);
var sumz = sumy(7);
console.log(sumz(13)); 
// => 25

类似地，局部应用的意思是一次对一个函数应用几个参数，然后返回另一个应用更多参数的函数。 以下为完整示例代码：

function sum(x, y, z) {
  return x + y + z;
}
var sumn = sum.bind(this, 1, 11);
console.log(sumn(23)); 
// => 35

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
