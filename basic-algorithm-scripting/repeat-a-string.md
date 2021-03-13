---
id: 604bfce02736d3312bd46a89
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 按指定数次重复一个字符串
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

按指定数次重复一个字符串

今天我们通过两种方法将一个字符串重复自身 N 次。在介绍实现方法之前，我们再熟悉下数组的 join() 方法和字符串的 repeat() 方法。

join() 方法将一个数组（或一个类数组对象）的所有元素连接成一个字符串并返回这个字符串。如果数组只有一个项目，那么将返回该项目而不使用分隔符。

语法：

arr.join([separator])

参数：

separator 可选，指定一个字符串来分隔数组的每个元素。如果需要，将分隔符转换为字符串。如果缺省该值，数组元素用逗号（,）分隔。如果 separator 是空字符串("")，则所有元素之间都没有任何字符。

返回值：一个所有数组元素连接的字符串。如果 arr.length 为0，则返回空字符串。

repeat() 构造并返回一个新字符串，该字符串包含被连接在一起的指定数量的字符串的副本。

语法：

str.repeat(count)

参数：

count   介于 0 和 +Infinity 之间的整数。表示在新构造的字符串中重复了多少遍原字符串


返回值：包含指定字符串的指定数量副本的新字符串。


第一种方法：使用 while 循环重复字符串，执行步骤如下所示：

1、当执行次数大于零时，while 语句执行

2、将要重复的字符串添加至数组

3、重复次数减1

4、通过 '' 分隔符连接数组内容为字符串，返回结果字符串 

function repeatStr(str, times) {
  var repeatedStrs = [];
  while (times > 0) {
    repeatedStrs.push(str);
    times--;
  }
  return repeatedStrs.join('');
}

console.log( repeatStr('路条编程',3) );
// => 路条编程路条编程路条编程

第二种方法：使用 ES6 repeat()方法重复一个字符串，执行步骤如下所示：

1、判断执行次数是否大于零

2、大于零返回字符串重复方法后的结果字符串

3、小于零返回空字符串

function repeatStr2(str, times) {

  if (times > 0) {
    return str.repeat(times); 
  }
  else {
    return "";
  }
}
console.log( repeatStr2('路条编程',5) );
// => 路条编程路条编程路条编程路条编程路条编程


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
