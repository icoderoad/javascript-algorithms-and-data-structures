---
id: 602dfd07fc10a8b926bdef6b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用方括号访问数组的内容
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用方括号访问数组的内容

所有数据结构的基本特性是，它们不仅能够存储数据，我们还能够按照需求来访问存放在其中的数据。上篇文章中我们已经学习了如何创建一个数组结构，现在让我们开始学习如何访问这个数组结构中的数据。

我们先定义一个包含 3 个元素的数组：

let mArr = ["路条", "编程", "欢迎您！"];

在一个数组结构中，其内部的每个元素都有一个与之对应的索引（index）。索引是该元素在数组中的位置，可被用于引用该元素。但需要注意的是，JavaScript 语言中数组的索引是从 0 开始的（zero-indexed），即一个数组的第一个元素是在数组中的第 0 个位置，而不是第 1 个位置。 

要从一个数组中获取一个元素，我们可以在一个数组变量名的后面加一个使用“方括号”括起来的索引。这叫做方括号符号（bracket notation）。 

例如我们要从 mArr 数组变量中获取数据元素 "路条" 并将其赋值给一个变量，我们可以编写如下所示的代码：

let mArr = ["路条", "编程", "欢迎您！"];
let mEle = mArr[0];
console.log( mEle );
// => 路条

除了使用 “索引” 来获取某个元素值以外，您还可以通过类似的方法来设置一个索引位置所对应的元素值：

mArr[1] = "公众号";
console.log( mArr );
// => (3) ["路条", "公众号", "欢迎您！"]

在控制台执行以上代码，我们通过控制台的输出结果可知，我们已经通过方括号将索引为 1 的元素从 "编程" 设置为了 "公众号"。


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
