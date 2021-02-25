---
id: 603756e90973394a08f677e0
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 For 循环迭代数组的所有项
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 For 循环迭代数组的所有项

在进行与数组有关的编程时，我们有时需要遍历数组的所有元素来找出我们需要的元素，或者对数组执行特定的操作。JavaScript 语言提供了几个内置的方法，它们以不同的方式遍历数组来获得不同的结果（如every()、forEach()、map()等等）。而简单的 for 循环不仅能实现这些功能，而且相比之下也更灵活。

for 语句用于创建一个循环，它包含了三个可选的表达式，这三个表达式被包围在圆括号之中，使用分号分隔，后跟一个用于在循环中执行的语句（通常是一个块语句）。

语法：

for ([initialization]; [condition]; [final-expression])
   statement

参数：

initialization

一个表达式 (包含赋值语句) 或者变量声明。典型地被用于初始化一个计数器。该表达式可以使用 var 或 let 关键字声明新的变量，使用 var 声明的变量不是该循环的局部变量，而是与 for 循环处在同样的作用域中。用 let 声明的变量是语句的局部变量。该表达式的结果无意义。

condition

一个条件表达式被用于确定每一次循环是否能被执行。如果该表达式的结果为 true，statement 将被执行。这个表达式是可选的。如果被忽略，那么就被认为永远为真。如果计算结果为假，那么执行流程将被跳到 for 语句结构后面的第一条语句。

final-expression

每次循环的最后都要执行的表达式。执行时机是在下一次 condition 的计算之前。通常被用于更新或者递增计数器变量。
statement

只要 condition 的结果为 true 就会被执行的语句。要在循环体内执行多条语句，使用一个块语句（{ ... }）来包含要执行的语句。没有任何语句要执行，使用一个空语句（;）。

请看以下例子：

function greaterThanNum(arr, num) {
  let newArr = [];
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] > num) {
      newArr.push(arr[i]);
    }
  }
  return newArr;
}

let numArr = greaterThanNum([32, 12, 68, 54, 80, 0, 1], 22);
console.log( numArr );
// => (4) [32, 68, 54, 80]

这个函数使用一个 for 循环来遍历一个数组，逐一对其中的元素进行测试。我们用这个方法简单地以编程的方式找出了数组中大于变量 num  的元素，并返回了一个包含这些元素的数组。

下面我们做个复杂一点的练习，我们定义一个返回数组包含指定元素的函数，它接受一个嵌套的数组参数 arr 以及一个 ele 参数，并要返回一个新数组。arr 数组中的数组可能包含 ele 元素，也可能不包含。最终函数返回一个由 arr 中不包含 ele 的数组组成的新数组。

function getContainsArray(arr, ele) {
  let eleArr = [];

  for (let i = 0; i < arr.length; i++) {
    if (arr[i].includes(ele)) {
      eleArr.push(arr[i]);
    }
  }

  return eleArr;
}

console.log(getContainsArray([['路条科技', '阿里', '腾讯'], ['微信公众号', '路条公众号', '美团公众号'], ['万科集团', '绿地集团', '保利集团'], ['头条', '路条', '苹果']], '路条'));

// => (3) ["头条", "路条", "苹果"]


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
