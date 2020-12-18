---
id: 5fdc3d5856043c8366f5fe21
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 操作复杂对象和嵌套对象
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
操作复杂对象和嵌套对象。

有时你可能希望将数据存储在灵活的数据结构中。JavaScript 对象是处理灵活数据的一种方法。它可以储存字符串、数字、布尔值、函数和对象以及这些值的任意组合。

这是一个复杂数据结构的示例：

var musicArr = [
  {
    "artist": "是七叔呢",
    "title": "踏山河",
    "release_year": 2020,
    "formats": [ 
      "AAC", 
      "MP3"
    ],
    "gold": true
  }
];

这是一个对象数组，并且对象有各种关于音乐的详细信息。它也有一个嵌套的 formats 的数组。附加单曲音频格式可以被添加到数组中。 对象将数据以一种键-值对的形式保存。在上面的示例中，"artist": "七叔呢" 是一个具有 "artist" 键和 "七叔呢" 值的属性。 

JavaScript Object Notation 简称 JSON 是用于存储数据的相关数据交换格式。

{
    "artist": "是七叔呢",
    "title": "踏山河",
    "release_year": 2020,
    "formats": [ 
      "AAC", 
      "MP3"
    ],
    "gold": true
}

提示：数组中有多个 JSON 对象的时候，对象与对象之间要用逗号隔开。

前面我们介绍过通过串联点操作符或中括号操作符来访问简单对象属性，也可以通过这两个操作符访问对象的嵌套属性。

下面是一个嵌套的动物对象：

var animal = {
  "dog": {
    "name": "秋刀鱼"
  },
  "cat": {
    "body": { 
      "tails": 1,
      "legs": 4
    },
    "name": "哆啦A梦"
  }
};

console.log( animal.cat["body"].tails ) ; // 1
console.log( animal.dog.name ) ; // => 秋刀鱼

以上代码通过点操作符读取 cat属性，在 cat 属性下通过中括号读取 body 下 tails 属性值，控制台输出 1。 读取 dog 属性下的 name 属性，控制台输出的属性值为 秋刀鱼。

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
