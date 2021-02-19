---
id: 602f4f5dc27e616d28f8b748
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 push() 和 unshift() 添加元素到数组中
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 push() 和 unshift() 添加元素到数组中

一个数组的长度与其包含的数据类型一样，是不固定的。数组可以包含任意数量的元素，可以不限次数地往数组中添加元素或者从中移除元素，或者说数组是可变的。在本文中，我们要学习两个以编程方式修改数组的方法：Array.push() 和 Array.unshift() 。

push() 方法将一个或多个元素添加到数组的末尾，并返回该数组的新长度。

语法：arr.push(element1, ..., elementN)

参数：elementN 被添加到数组末尾的元素。

返回值：当调用该方法时，新的 length 属性值将被返回。

push 方法根据 length 属性来决定从哪里开始插入给定的值。如果 length 不能被转成一个数值，则插入的元素索引为 0，包括 length 不存在时。当 length 不存在时，将会创建它。

unshift() 方法将一个或多个元素添加到数组的开头，并返回该数组的新长度(该方法修改原有数组)。

语法：arr.unshift(element1, ..., elementN)

参数：elementN 要添加到数组开头的元素或多个元素。

返回值：当一个对象调用该方法时，返回其 length 属性值。

unshift 特意被设计成具有通用性；这个方法能够通过 call 或 apply 方法作用于类数组对象上。不过对于没有 length 属性（代表从0开始的一系列连续的数字属性的最后一个）的对象，调用该方法可能没有任何意义。

注意：如果传入多个参数，它们会被以块的形式插入到对象的开始位置，它们的顺序和被作为参数传入时的顺序一致。 于是，传入多个参数调用一次 unshift ，和传入一个参数调用多次 unshift (例如，循环调用)，它们将得到不同的结果


如下所示，push() 和 unshift() 这两个方法都接收一个或多个元素作为参数；对一个数组调用这两个方法都可以将输入的元素插入到该数组中。

push() 方法将元素插入到一个数组的末尾，而 unshift() 方法将元素插入到一个数组的开头。请看以下示例：

let welcomeMsg = '您好';
let strArr = ['路条编程', '欢迎您！'];

strArr.unshift('菜鸟', '001');
console.log( strArr );
// => (4) ["菜鸟", "001", "路条编程", "欢迎您！"]


strArr.push(welcomeMsg);
console.log( strArr );
// => (5) ["菜鸟", "001", "路条编程", "欢迎您！", "您好"]

以上代码我们先设置了一个变量 welcomeMsg 和 strArr， 第一个变量为字符串，第二个变量为字符串数组。我们对数组变量 strArr 调用 unshift() 方法后，在控制台打印输出数组，控制台输出添加元素后的数据。根据以上输出结果可知， unshift() 方法添加的两个元素被添加到了数组开头。我们再次调用 push()
方法，将变量 welcomeMsg 添加到数组并打印输出数组至控制台。根据以上输出结果可知，welcomeMsg 变量数组被添加到了数组结尾。

注意:我们还可以为数组 strArr 添加变量 welcomeMsg ，这允许我们很灵活地动态改变我们数组中的数据。




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
