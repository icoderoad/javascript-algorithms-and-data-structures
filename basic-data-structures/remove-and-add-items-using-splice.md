---
id: 6031fde23bb3109a693c9faf
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 splice() 删除和添加元素
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 splice() 删除和添加元素

在前面的文章中，我们已经学到了如何利用 shift() 和 pop() 方法从数组的开头或者末尾移除元素，但如果我们想移除数组中间的一个元素呢？或者想一次移除多个元素呢？这时候我们就需要 splice() 方法了。splice() 方法让我们可以从数组中的任意位置移除任意数量的连续的元素。

splice() 方法通过删除或替换现有元素或者原地添加新的元素来修改数组,并以数组形式返回被修改的内容。此方法会改变原数组。

语法：array.splice(start[, deleteCount[, item1[, item2[, ...]]]])

参数：

start​ 指定修改的开始位置（从 0 计数）。如果超出了数组的长度，则从数组末尾开始添加内容；如果是负值，则表示从数组末位开始的第几位（从 -1 计数，这意味着 -n 是倒数第 n 个元素并且等价于 array.length-n ）；如果负数的绝对值大于数组的长度，则表示开始位置为第 0 位。

deleteCount 可选，整数，表示要移除的数组元素的个数。

如果 deleteCount 大于 start 之后的元素的总数，则从 start 后面的元素都将被删除（含第 start 位）。
如果 deleteCount 被省略了，或者它的值大于等于 array.length - start (也就是说，如果它大于或者等于 start 之后的所有元素的数量)，那么 start 之后数组的所有元素都会被删除。
如果 deleteCount 是 0 或者负数，则不移除元素。这种情况下，至少应添加一个新元素。

item1, item2, ... 可选，要添加进数组的元素,从 start 位置开始。如果不指定，则 splice() 将只删除数组元素。

返回值：由被删除的元素组成的一个数组。如果只删除了一个元素，则返回只包含一个元素的数组。如果没有删除元素，则返回空数组。


经过上面的语法介绍，我们知道 splice() 方法最多可以接受 3 个参数，但现在我们先关注前两个。splice() 方法接收的前两个参数基于调用 splice()数组中元素的索引。记住，数组的索引是从 0 开始的，所以我们要用 0 来指示数组中的第一个元素。splice() 方法的第一个参数代表从数组中的哪个索引开始移除元素，而第二个参数指示要从数组中删除多少个元素。例如：

let mArr = ['您好', '菜鸟008', '路条', '编程', '欢迎您！'];

let delArr = mArr.splice(2, 2);
console.log( delArr );
// => (2) ["路条", "编程"] 

console.log( mArr );
// =>  (3) ["您好", "菜鸟008", "欢迎您！"]

以上代码我们定义了一个 5 个元素的数组 mArr， 调用数组 splice() 方法， 从第 3 个索引位置开始移除 2 个元素，将删除元素组成的数组赋值给变量 delArr， 在控制台打印输出删除数组元素，控制台输出为 “(2) ["路条", "编程"] ”。下行在控制台输出原数组 mArr， 控制台显示结果为 “(3) ["您好", "菜鸟008", "欢迎您！"]”，表示 splice（）方法已经成功删除 2 个元素。


上面我们介绍了 splice（）方法前两个参数的用法。现在来介绍 splice() 方法后面参数的用法。我们可以利用它的第三个参数来向数组中添加元素。第三个参数可以是一个或多个元素，这些元素会被添加到数组中。这使我们能够便捷地将数组中的一个或一系列元素换成其他的元素。我们在上面的示例基础上继续操作数组 mArr, 代码如下所示：

const start = 2;
const delNum = 1;

delArr = mArr.splice(start, delNum, 'welcome', 'to', 'www', 'icoderoad','.com!');
console.log( delArr );
// => ["欢迎您！"] 

console.log( mArr );
// =>  ["您好", "菜鸟008", "welcome", "to", "www", "icoderoad", ".com!"]

以上代码定义开始位置 start 为 2，删除元素数量 delNum 为 1， 接着调用 splice() 方法，在 (2) 的索引位置开始删除元素，删除的元素数量是 1，('welcome', 'to', 'www', 'icoderoad','.com!') 是在删除位置插入的元素，将删除元素赋值给变量 delArr , 控制台输出 ["欢迎您！"] ， 最后打印操作完成后的数组 mArr，控制台输出 ["您好", "菜鸟008", "welcome", "to", "www", "icoderoad", ".com!"] 。 

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
