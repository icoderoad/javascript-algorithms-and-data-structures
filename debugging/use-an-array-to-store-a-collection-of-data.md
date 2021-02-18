---
id: 602ba8da27bc4ca24ca69a2a
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组存储数据集合
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用数组存储数据集合

以下是数组（Array）数据结构的最简单的实现例子。这是一个一维数组（one-dimensional array），它只有一层，或者说在它里面没有包含其它的数组结构。可以看到它里面包含了布尔值（booleans）、字符串（strings）、数字（numbers）以及一些其他的 JavaScript 语言中合法的数据类型：

let arr = ['one', 2, 'three', true, false, undefined, null];
console.log(arr.length);
// =>  7

在上述例子中我们可以看到，所有数组都有一个长度（length）属性。可以简单地使用 Array.length 方法来访问它。 下面是一个关于数组的更复杂的例子。这是一个多维数组（multi-dimensional Array），或者说是一个包含了其他数组的数组。可以注意到，在它的内部还包含了 JavaScript 语言中的对象（objects）结构。我们会在后面的文章中讨论该数据结构，但现在您只需要知道数组能够存储复杂的对象类型数据。

let complexArray = [
  [
    {
      one: 1,
      two: 2
    },
    {
      three: 3,
      four: 4
    }
  ],
  [
    {
      a: "a",
      b: "b"
    },
    {
      c: "c",
      d: "d"
    }
  ]
];

下面我们来做个练习，我们已经定义了一个名为 mArr 的变量。将一个含有至少 5 个元素的数组赋值给 mArr 变量。数组 mArr 应该包含至少一个 string 类型的数据、一个 number 类型的数据和一个 boolean 类型的数据。代码如下所示：

let mArr;
mArr = ["路条编程", 2021, true, "www.icoderoad.com", "欢迎您！"]
console.log( mArr );
// => (5) ["路条编程", 2021, true, "www.icoderoad.com", "欢迎您！"]

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
