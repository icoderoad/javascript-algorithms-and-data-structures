---
id: 604ef093e49cf062c9f7fd0c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 字符串单词首字母大写的实现方法
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

字符串单词首字母大写的实现方法

今天我们介绍字符串单词首字母大写的实现方法。此方法返回提供的字符串每个单词的首字母大写，其余部分为小写。在介绍具体方法之前，我们先介绍下字符串的 substr() 方法、 toUpperCase() 方法和 toLowerCase()。

substr() 方法返回一个字符串中从指定位置开始到指定字符数的字符。

语法：

str.substr(start[, length])

参数：

start 	开始提取字符的位置。如果为负值，则被看作 strLength + start，其中 strLength 为字符串的长度（例如，如果 start 为 -3，则被看作 strLength + (-3)）。

length 	可选。提取的字符数。


start 是一个字符的索引。首字符的索引为 0，最后一个字符的索引为 字符串的长度减去1。substr 从 start 位置开始提取字符，提取 length 个字符（或直到字符串的末尾）。

如果 start 为正值，且大于或等于字符串的长度，则 substr 返回一个空字符串。

如果 start 为负值，则 substr 把它作为从字符串末尾开始的一个字符索引。如果 start 为负值且 abs(start) 大于字符串的长度，则 substr 使用 0 作为开始提取的索引。注意负的 start 参数不被 Microsoft JScript 所支持。

如果 length 为 0 或负值，则 substr 返回一个空字符串。如果忽略 length，则 substr 提取字符，直到字符串末尾。

toUpperCase() 方法将调用该方法的字符串转为大写形式并返回（如果调用该方法的值不是字符串类型会被强制转换）。

语法：

str.toUpperCase()

返回值：

一个新的字符串，表示转换为大写的调用字符串。

toLowerCase() 会将调用该方法的字符串值转为小写形式，并返回。

语法：

str.toLowerCase()

返回值：

一个新的字符串，表示转换为小写的调用字符串。

算法实现步骤如下所示：

1、将字符串按格式分隔为数组

2、通过循环遍历数组

3、每次迭代取出一个数组元素，赋值给一个临时变量

4、对临时变量第一个字母进行大写转换，对除首字母们的字符进行小写处理并拼接为新的字符串

5、将临时变量替换之前的数组元素

6、将数组转换为字符串返回


function titleCase(str) {
  var arrs = str.split(' ');
  for(var i=0; i<arrs.length;i++){
    var tmpVal = arrs[i];
    tmpVal = tmpVal.substr(0,1).toUpperCase() +tmpVal.substr(1).toLowerCase();
    arrs[i] = tmpVal;
  }
  return arrs.join( ' ' );
}


// 今日事须今日毕，切勿拖延到明天。
console.log(titleCase('Never deter till tomorrow that which you can do today.'));
// => Never Deter Till Tomorrow That Which You Can Do Today.

//万物皆有时，时来不可失。
console.log(titleCase('Everything has its time and that time must be watched.'));
// => Everything Has Its Time And That Time Must Be Watched.


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
