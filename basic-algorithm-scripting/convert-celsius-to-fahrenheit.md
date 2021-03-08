---
id: 6041c1929fc8764ca0a36424
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将摄氏温度转换为华氏温度
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

将摄氏温度转换为华氏温度

从今天开始，我们做一些综合的练习，今天我们介绍一个温度转换的方法。从摄氏温度转换为华氏温度的算法是以摄氏度乘以 9/5，再加上 32 。您将获得一个参数 celsius 代表摄氏温度。使用已准备好代表华氏温度的变量 fahrenheit，将 celsius 摄氏温度变量值转换成华氏温度值，然后存储在 farenheit 变量里。使用以上提到的算法将摄氏温度转换为华氏温度。根据算法可知，先将参数 celsius 乘以 9/5，在 JavaScript 语句中，乘法运算符使用星号(*) ，由于乘以一个分数，所以将分数使用小括号括起来, 然后再加 32，最终算法如下所示： 

function convertToF(celsius) {
  let fahrenheit;
  fahrenheit = celsius * (9/5) + 32;
  return fahrenheit;
}

let fVal = convertToF(-40);
console.log( fVal );
// => -40

fVal = convertToF(-20);
console.log( fVal );
// => -4

fVal = convertToF(0);
console.log( fVal );
// => 32

fVal = convertToF(20);
console.log( fVal );
// => 68

fVal = convertToF(40);
console.log( fVal );
// => 104

以上代码我们调用了转换方法 convertToF， 分别设置摄氏温度为 -40、-20、0、20、40， 转换后的华氏温度在控制台打印输出，华氏温度值分别为 -40、-4、32、68、104。


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
