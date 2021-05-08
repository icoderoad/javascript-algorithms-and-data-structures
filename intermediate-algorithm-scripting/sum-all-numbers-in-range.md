---
id: 60961647ba50c85eb90c93fe
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: JavaScript 中的函数柯里化
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

指定范围内的数字求和

从今天开始，我们介绍一些算法相关的示例。本次练习需要写一个方法，该方法将一个含有两个数字的数组，让它返回这两个数字间所有数字（包含这两个数字）的总和。

例如，sumAllNumberArr([4,1]) 应该返回 10，因为从 1 到 4 （包含 1、4）的所有数字的和是 10。

在介绍完整代码之前，我们先介绍下 Math.min() 和 Math.max() 的具体用法：

Math.min() 返回零个或更多个数值的最小值。

语法：
Math.min([value1[,value2, ...]]) 

参数：
value1, value2, ... 一组数值

返回值：
给定数值中最小的数。如果任一参数不能转换为数值，则返回NaN。

Math.max() 函数返回一组数中的最大值。

语法：
Math.max(value1[,value2, ...]) 

参数：
value1, value2, ... 一组数值

返回值：
返回给定的一组数字中的最大值。如果给定的参数中至少有一个参数无法被转换成数字，则会返回 NaN。

我们定义一个方法 sumAllNumberArr， 参数为一个数字数组 arr ，该方法返回结果为求和后的数字。具体代码如下所示：

function  sumAllNumberArr( arr ){
  let total = 0;
  for (let i = Math.min(...arr); i <= Math.max(...arr); i++) {
    total += i;
  }
  return total;
}

var total = sumAllNumberArr([3, 8]);
console.log(total);
// => 33
 

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
