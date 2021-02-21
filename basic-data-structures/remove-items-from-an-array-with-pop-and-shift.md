---
id: 6030a0a0d82bca435ecc1d63
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 pop() 和 shift() 从数组中删除项目
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 pop() 和 shift() 从数组中删除项目

push() 和 unshift() 都分别有一个作用基本与之相反的方法：pop() 和 shift()。根据方法名称或许您已经猜到，与插入元素相反，pop() 从数组的末尾移除一个元素，而 shift() 从数组的开头移除一个元素。pop() 和 shift() 与对应的 push() 和 unshift() 的关键区别在于，前者不能接受输入参数，而且每次只能修改数组中的一个元素。

pop() 方法从数组中删除最后一个元素，并返回该元素的值。此方法更改数组的长度。

语法：arr.pop()

返回值：从数组中删除的元素(当数组为空时返回 undefined )。

pop 方法有意具有通用性。该方法和 call() 或 apply() 一起使用时，可应用在类似数组的对象上。pop 方法根据 length 属性来确定最后一个元素的位置。如果不包含 length 属性或 length 属性不能被转成一个数值，会将 length 置为 0，并返回 undefined。

shift() 方法从数组中删除第一个元素，并返回该元素的值。此方法更改数组的长度。

语法：arr.shift()

返回值：从数组中删除的元素; 如果数组为空则返回undefined 。 

shift 方法移除索引为 0 的元素(即第一个元素)，并返回被移除的元素，其他元素的索引值随之减 1。如果 length 属性的值为 0 (长度为 0)，则返回 undefined。

shift 方法并不局限于数组：这个方法能够通过 call 或 apply 方法作用于类似数组的对象上。但是对于没有 length 属性（从 0 开始的一系列连续的数字属性的最后一个）的对象，调用该方法可能没有任何意义。


让我们来看以下的例子：

let welcomeMsgs = ['您好', '菜鸟001', '欢迎访问路条编程网站!'];

let msg = welcomeMsgs.pop();
console.log(msg);
// => 欢迎访问路条编程网站!

console.log(welcomeMsgs);
// => (2) ["您好", "菜鸟001"]

msg = welcomeMsgs.shift();
console.log(msg);
// => 您好

console.log(welcomeMsgs);
// => ["菜鸟001"]

以上代码我们将数组赋值给变量 welcomeMsgs， 调用 pop 方法，将被移除的元素赋值给变量 msg ，在控制台输出变量 msg 值，控制台输出 “欢迎访问路条编程网站!”。说明 pop 方法删除数组中的最后一个元素。然后在控制台输出 welcomeMsgs 数组，控制台显示 “(2) ["您好", "菜鸟001"]”，说明最后元素被删除成功。接下来调用 shift 方法，并将删除元素赋值给变量 msg , 在控制台输出 msg 结果为 “您好”，说明 shift 方法已经删除数组中第一个元素，再次在控制台打印 welcomeMsgs 数组，输出结果为 “["菜鸟001"]” ，说明数组第一个元素已经删除成功。


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
