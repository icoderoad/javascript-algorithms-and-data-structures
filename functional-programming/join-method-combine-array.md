---
id: 6090aaca13e3ed998cb047c7
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组 join() 方法将数组组合成字符串
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组 join() 方法将数组组合成字符串

join() 方法用来把数组中的所有元素放入一个字符串，并通过指定的分隔符参数进行分隔。在练习示例之前，先介绍下 join() 方法的具体用法。


join() 方法将一个数组（或一个类数组对象）的所有元素连接成一个字符串并返回这个字符串。如果数组只有一个项目，那么将返回该项目而不使用分隔符。 

语法：
arr.join([separator])

参数：
separator 可选，指定一个字符串来分隔数组的每个元素。如果需要，将分隔符转换为字符串。如果缺省该值，数组元素用逗号（,）分隔。如果separator是空字符串("")，则所有元素之间都没有任何字符。

返回值：
一个所有数组元素连接的字符串。如果 arr.length 为 0，则返回空字符串。

描述：
所有的数组元素被转换成字符串，再用一个分隔符将这些字符串连接起来。

注意：如果一个元素为 undefined 或 null，它会被转换为空字符串。

举个例子：

var arr = ["路条编程", "欢迎您！"];
var wlecomeArrs = arr.join("，");
console.log( wlecomeArrs )
// => 路条编程，欢迎您！

我们练习一个完整的示例，定义一个方法 strToSentence, 包含一个参数 str， 方法内用 join 方法（及其他方法）将字符串 str 中的单词组成句子，这个方法返回一个字符串。举个例子，"我-喜欢-在-路条编程-网站-练习-编程！" 会被转换成 "我喜欢在路条编程网站练习编程！"。在此方法中不能使用字符串的 replace 方法。

function strToSentence(str) {
 	return str.split(/[-\,.]/).join("");
}

console.log(strToSentence("我-喜欢-在-路条编程-网站-练习-编程！"));
// => 我喜欢在路条编程网站练习编程！

console.log(strToSentence("编程,菜鸟,路条编程,欢迎您！"));
// => 编程菜鸟路条编程欢迎您！

console.log(strToSentence("路条编程.不仅.是.在线学习.编程.的.平台，也是.学习.编程.的.友好社区！"));
// => 路条编程不仅是在线学习编程的平台，也是学习编程的友好社区！

以上代码方法 strToSentence 中分隔字符串使用了 split 的正则规则，按-或,和.分隔为字符串数组，再通过数组 join() 方法将数组组合成一个字符串。




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
