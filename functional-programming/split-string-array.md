---
id: 6090aaca13e3ed998cb047c7
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用字符串 join 方法将数组组合成字符串
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用字符串 split 方法将字符串拆分成数组

字符串 split 方法用于把字符串分割成字符串数组，接收一个分隔符参数，分隔符可以是用于分解字符串或正则表达式的字符。在练习示例之前，先介绍下 split 方法的具体用法。

split() 方法使用指定的分隔符字符串将一个String对象分割成子字符串数组，以一个指定的分割字串来决定每个拆分的位置。 

语法：
str.split([separator[, limit]])

注意：如果使用空字符串(“)作为分隔符，则字符串不是在每个用户感知的字符(图形素集群)之间，也不是在每个Unicode字符(代码点)之间，而是在每个UTF-16代码单元之间。这会摧毁代理对。还请参见how do you get a string to a character array in javascript

参数：
separator

	指定表示每个拆分应发生的点的字符串。separator 可以是一个字符串或正则表达式。 如果纯文本分隔符包含多个字符，则必须找到整个字符串来表示分割点。如果在str中省略或不出现分隔符，则返回的数组包含一个由整个字符串组成的元素。如果分隔符为空字符串，则将str原字符串中每个字符的数组形式返回。

limit
	一个整数，限定返回的分割片段数量。当提供此参数时，split 方法会在指定分隔符的每次出现时分割该字符串，但在限制条目已放入数组时停止。如果在达到指定限制之前达到字符串的末尾，它可能仍然包含少于限制的条目。新数组中不返回剩下的文本。

返回值：
	返回源字符串以分隔符出现位置分隔而成的一个 Array 

描述：
	找到分隔符后，将其从字符串中删除，并将子字符串的数组返回。如果没有找到或者省略了分隔符，则该数组包含一个由整个字符串组成的元素。如果分隔符为空字符串，则将str转换为字符数组。如果分隔符出现在字符串的开始或结尾，或两者都分开，分别以空字符串开头，结尾或两者开始和结束。因此，如果字符串仅由一个分隔符实例组成，则该数组由两个空字符串组成。

	如果分隔符是包含捕获括号的正则表达式，则每次分隔符匹配时，捕获括号的结果（包括任何未定义的结果）将被拼接到输出数组中。但是，并不是所有浏览器都支持此功能。


举个例子，如果分隔符是空格，将会得到一个单词数组；如果分隔符是空字符串，会得到一个由字符串中每个字符组成的数组。

下面是的示例一个是用分号分隔一个字符串的例子，另一个是用数字的正则表达式分隔的示例。具体代码如下所示：

var welcomeMsg = "您好，欢迎光临路条编程网站！";
var msgArrs = welcomeMsg.split("，");
console.log( msgArrs );
// => (2) ["您好", "欢迎光临路条编程网站！"]

var welcomeMsg2 = "您好9路条7编程网站2欢迎您!";
var msgArrs2 = welcomeMsg2.split(/\d/);
console.log( msgArrs2 );
// => (4) ["您好", "路条", "编程网站", "欢迎您!"]

因为字符串是固定的，split 方法可以更简单的操作它们。

下面我们练习一个完整的示例，我们定义一个 strSplit 方法，方法包含一个参数 str, 方法用 split 方法将 str 分割成单词数组，这个方法应该返回一个数组。单词不一定都是用空格分隔，所以数组中不应包含标点符号。

function strSplit(str) {
  return str.split(/\W/);
}
console.log( strSplit("Hello coder,I-am icoderoad.com"));
// => (6) ["Hello", "coder", "I", "am", "icoderoad", "com"] 




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
