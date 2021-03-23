---
id: 605536345ef9cd6dd129287b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 判断数组的第一个元素中的字符串是否包含数组第二个元素中字符串的所有字符
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

判断数组的第一个元素中的字符串是否包含数组第二个元素中字符串的所有字符

今天我们介绍判断数组的第一个元素中的字符串是否包含数组第二个元素中字符串的所有字符方法。在介绍具体方法之前，我们先介绍下字符串的 indexOf()、和 toLowerCase() 方法。

indexOf() 方法返回调用它的 String 对象中第一次出现的指定值的索引，从 fromIndex 处进行搜索。如果未找到该值，则返回 -1。

语法：

str.indexOf(searchValue [, fromIndex])

参数：
searchValue 要被查找的字符串值。

如果没有提供确切地提供字符串，searchValue 会被强制设置为 "undefined"， 然后在当前字符串中查找这个值。

数字表示开始查找的位置。可以是任意整数，默认值为 0。

如果 fromIndex 的值小于 0，或者大于 str.length ，那么查找分别从 0 和 str.length 开始。（译者注：  fromIndex 的值小于 0，等同于为空情况； fromIndex 的值大于或等于 str.length ，那么结果会直接返回 -1 。）

返回值：

查找的字符串 searchValue 的第一次出现的索引，如果没有找到，则返回 -1。

toLowerCase() 会将调用该方法的字符串值转为小写形式，并返回。

语法：

str.toLowerCase()

返回值：

一个新的字符串，表示转换为小写的调用字符串。

实现步骤如下所示：

1、将数组的第一个元素和第二个元素转换小写后赋值给两个变量 str1、str2

2、初始化计数变量为 0 

3、使用 for 循环遍历搜索字符串的每个字符

4、 如果字符串中包含搜索字符串中的字符，计数变量 + 1

5、判断计数变量与搜索字符串长度是否一至，是则返回 true， 否则返回 false;

具体代码如下所示：

function checkStringContainsAllSearchStr( arr ) {
	var str1 = arr[0].toLowerCase();
    var str2 = arr[1].toLowerCase();
    var num = 0;
    for(var i = 0; i < str2.length; i++){
      if(str1.indexOf(str2[i]) !== -1){
        num++;
      }
    }
    if( str2.length === num ) {
      return true;
    }else{
      return false;
    }
}

console.log( checkStringContainsAllSearchStr(["路条编程网站", "路条"]) );
// => true

console.log( checkStringContainsAllSearchStr(["www.icoderoad.com","icoderoad"]) );
// => true

console.log( checkStringContainsAllSearchStr(["您好，编程小白","路条"]) );
// => false

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
