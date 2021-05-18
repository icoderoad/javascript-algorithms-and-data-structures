---
id: 60a210e93da8e91fbec0dc3f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 查找传入的字符串里缺失的字母
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

查找传入的字符串里缺失的字母

本次练习我们需要写一个函数 findMissingLetters 。该方法接收一个参数 str，该方法找到传入的字符串里缺失的字母并返回它。

判断缺失的依据是字母顺序，比如 abcdfg 中缺失了 e。而 abcdef 中就没有字母缺失，此时我们需要返回 undefined。


在介绍完整代码之前，我们先介绍下字符串 charCodeAt 和  fromCharCode 方法的具体用法： 

charCodeAt() 方法返回 0 到 65535 之间的整数，表示给定索引处的 UTF-16 代码单元

语法：
str.charCodeAt(index)

参数：
index 一个大于等于 0，小于字符串长度的整数。如果不是一个数值，则默认为 0。

返回值：
指定 index 处字符的 UTF-16 代码单元值的一个数字；如果 index 超出范围，charCodeAt() 返回 NaN。

fromCharCode() 方法返回由指定的 UTF-16 代码单元序列创建的字符串。

语法：
String.fromCharCode(num1[, ...[, numN]])

参数：
num1, ..., numN 一系列 UTF-16 代码单元的数字。范围介于 0 到 65535（0xFFFF）之间。大于 0xFFFF 的数字将被截断。不进行有效性检查。

返回值：
一个长度为 N 的字符串，由 N 个指定的 UTF-16 代码单元组成。

练习完整代码如下所示：

function findMissingLetters( str ){
  for (var i = 0; i < str.length; i++) {
    var code = str.charCodeAt(i);
   
    if (code !== str.charCodeAt(0) + i) {
      return String.fromCharCode(code - 1);
    }
  }
  return undefined;
}

console.log( findMissingLetters('stuwx') );
// => v


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
