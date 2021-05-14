---
id: 609e13995ce5abd1ee7aeb2c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将传入英语单词自动转换为英语黑话
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

将传入英语单词自动转换为英语黑话

本次练习我们需要写一个函数 strToPigLatin 。该方法接收一个参数 str，该方法把传入的字符串翻译成“英语黑话”。英语黑话”的基本转换规则很简单，只需要把一个英文单词的第一个辅音字母或第一组辅音簇移到单词的结尾，并在后面加上ay即可。在英语中，字母 a、e、i、o、u 为元音，其余的字母均为辅音。辅音簇的意思是连续的多个辅音字母。

额外地，如果单词本身是以元音开头的，那只需要在结尾加上way。

额外地，如果单词不包含元音，那只需要在结尾加上ay。

本次练习中，传入的单词一定会是英文单词，且所有字母均为小写。

在介绍完整代码之前，我们先介绍下字符串 match 和 substr 方法的具体用法： 

match() 方法检索返回一个字符串匹配正则表达式的结果。

语法：
str.match(regexp)

参数：
regexp 一个正则表达式对象。如果传入一个非正则表达式对象，则会隐式地使用 new RegExp(obj) 将其转换为一个 RegExp 。如果你没有给出任何参数并直接使用match() 方法 ，你将会得到一 个包含空字符串的 Array ：[""] 。

返回值：
如果使用g标志，则将返回与完整正则表达式匹配的所有结果，但不会返回捕获组。
如果未使用g标志，则仅返回第一个完整匹配及其相关的捕获组（Array）。 在这种情况下，返回的项目将具有如下所述的其他属性。

附加属性：
如上所述，匹配的结果包含如下所述的附加特性。

groups: 一个捕获组数组 或 undefined（如果没有定义命名捕获组）。
index: 匹配的结果的开始位置
input: 搜索的字符串.
一个Array，其内容取决于global（g）标志的存在与否，如果未找到匹配则为null。

substr() 方法返回一个字符串中从指定位置开始到指定字符数的字符。

语法：
str.substr(start[, length])

参数：
	start 开始提取字符的位置。如果为负值，则被看作 strLength + start，其中 strLength 为字符串的长度（例如，如果 start 为 -3，则被看作 strLength + (-3)）。
	length，可选。提取的字符数。


练习完整代码如下所示：

function strToPigLatin( str ){
  var pigLatin = "";
  var regex = /[aeiou]/gi;

  if (str[0].match(regex)) {
    pigLatin = str + "way";
  } else if (str.match(regex) === null) {
    pigLatin = str + "ay";
  } else {
    var vowelIndice = str.indexOf(str.match(regex)[0]);

    pigLatin = str.substr(vowelIndice) + str.substr(0, vowelIndice) + "ay";
  }

  return pigLatin;
}

console.log( strToPigLatin("icoderoad") );
// => icoderoadway


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
