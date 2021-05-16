---
id: 609e13995ce5abd1ee7aeb2c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 字符串的搜索与替换
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

字符串的搜索与替换

本次练习我们需要写一个函数 strSearchAndReplace 。该方法接收三个参数，它的返回值为完成替换后的新字符串。

这个函数接收的第一个参数为待替换的句子 str。

第二个参数为句中需要被替换的单词 sword。

第三个参数为替换后的单词 rword。

注意：您需要保留被替换单词首字母的大小写格式。即如果传入的第二个参数为 "jd"，第三个参数为 "icoderoad"，那么替换后的结果应为 "Icoderoad"

在介绍完整代码之前，我们先介绍下字符串 toUpperCase 和 replace 方法的具体用法： 

toUpperCase() 方法将调用该方法的字符串转为大写形式并返回（如果调用该方法的值不是字符串类型会被强制转换）。

语法:
str.toUpperCase()

返回值:
一个新的字符串，表示转换为大写的调用字符串。

replace() 方法返回一个由替换值（replacement）替换部分或所有的模式（pattern）匹配项后的新字符串。模式可以是一个字符串或者一个正则表达式，替换值可以是一个字符串或者一个每次匹配都要调用的回调函数。如果pattern是字符串，则仅替换第一个匹配项。

语法:
str.replace(regexp|substr, newSubStr|function)

参数:
  regexp (pattern)
    一个RegExp 对象或者其字面量。该正则所匹配的内容会被第二个参数的返回值替换掉。
  substr (pattern)
    一个将被 newSubStr 替换的 字符串。其被视为一整个字符串，而不是一个正则表达式。仅第一个匹配项会被替换。
  newSubStr (replacement)
    用于替换掉第一个参数在原字符串中的匹配部分的字符串。该字符串中可以内插一些特殊的变量名。参考下面的使用字符串作为参数。
  function (replacement)
    一个用来创建新子字符串的函数，该函数的返回值将替换掉第一个参数匹配到的结果。参考下面的指定一个函数作为参数。

返回值:
一个部分或全部匹配由替代模式所取代的新的字符串。


练习完整代码如下所示：

function strSearchAndReplace( str, sword , rword){
  if (/^[A-Z]/.test(sword)) {
    rword = rword[0].toUpperCase() + rword.substring(1)
  } else {
    rword = rword[0].toLowerCase() + rword.substring(1)
  }

  return str.replace(sword, rword);
}

console.log( strSearchAndReplace("welcome to Xxx.com", "Xxx", "icoderoad") );
// => welcome to Icoderoad.com 


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
