---
id: 609cba2f8ff0c76da2e03d61
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将字符串转换为短线连接格式
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

将字符串转换为短线连接格式

本次练习我们需要写一个函数 stringJoinCase 。该方法接收一个参数str，该方法返回处理后的字符串。把一个字符串转换为短线连接格式。短线连接格式的意思是，所有字母都是小写，且用-连接。比如，对于hello IcodeRoad，应该转换为hello-icoderoad；对于I love_Icoderoad-VeryMuch，应该转换为i-love-icoderoad-very-much。


在介绍完整代码之前，我们先介绍下字符串 split 和 toLowerCase 方法的具体用法： 

split() 方法使用指定的分隔符字符串将一个String对象分割成子字符串数组，以一个指定的分割字串来决定每个拆分的位置。 

语法：
str.split([separator[, limit]])

注意：如果使用空字符串(“)作为分隔符，则字符串不是在每个用户感知的字符(图形素集群)之间，也不是在每个Unicode字符(代码点)之间，而是在每个UTF-16代码单元之间。这会摧毁代理对。

参数：
separator，指定表示每个拆分应发生的点的字符串。separator 可以是一个字符串或正则表达式。 如果纯文本分隔符包含多个字符，则必须找到整个字符串来表示分割点。如果在str中省略或不出现分隔符，则返回的数组包含一个由整个字符串组成的元素。如果分隔符为空字符串，则将str原字符串中每个字符的数组形式返回。

limit 一个整数，限定返回的分割片段数量。当提供此参数时，split 方法会在指定分隔符的每次出现时分割该字符串，但在限制条目已放入数组时停止。如果在达到指定限制之前达到字符串的末尾，它可能仍然包含少于限制的条目。新数组中不返回剩下的文本。

返回值：
返回源字符串以分隔符出现位置分隔而成的一个 Array 

toLowerCase() 函式会回传将字符串转换为英文小写字母后的结果。

语法：
str.toLowerCase()

返回值：
回传一组将原字串英文内容转换成英文小写字母后的结果。

练习完整代码如下所示：

function stringJoinCase( str ){
  return str
    .split(/\s|_|(?=[A-Z])/)
    .join("-")
    .toLowerCase();
}

console.log( stringJoinCase("Welcome to Icoderoad.com!") );
// => welcome-to-icoderoad.com!


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
