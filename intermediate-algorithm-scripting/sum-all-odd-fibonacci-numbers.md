---
id: 60a62cbc9c3c44face1fca86
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 求斐波那契数组中的奇数之和

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

求斐波那契数组中的奇数之和

本次练习我们需要写一个函数 sumFibs，参数为一个正整数 num。它的作用是计算斐波那契数列中，小于或等于 num 的奇数之和。

斐波那契数列中，第一和第二个数字都是 1，后面的每个数字由之前两数相加得出。斐波那契数列的前六个数字分别为：1、1、2、3、5、8。

比如，sumFibs(10)应该返回10。因为斐波那契数列中，比10小的数字只有 1、1、3、5。


在介绍完整代码之前，我们先介绍下数组 unshift 方法和数组 reduce 方法的具体用法： 

unshift() 方法将一个或多个元素添加到数组的开头，并返回该数组的新长度(该方法修改原有数组)。

语法：
arr.unshift(element1, ..., elementN)

参数列表 elementN 要添加到数组开头的元素或多个元素。

返回值：
当一个对象调用该方法时，返回其 length 属性值。

reduce() 方法对数组中的每个元素执行一个由您提供的reducer函数(升序执行)，将其结果汇总为单个返回值。

reducer 函数接收4个参数:

Accumulator (acc) (累计器)
Current Value (cur) (当前值)
Current Index (idx) (当前索引)
Source Array (src) (源数组)
您的 reducer 函数的返回值分配给累计器，该返回值在数组的每个迭代中被记住，并最后成为最终的单个结果值。

语法：
arr.reduce(callback(accumulator, currentValue[, index[, array]])[, initialValue])

参数：
  callback
    执行数组中每个值 (如果没有提供 initialValue则第一个值除外)的函数，包含四个参数：
  accumulator
    累计器累计回调的返回值; 它是上一次调用回调时返回的累积值，或initialValue（见于下方）。

  currentValue
    数组中正在处理的元素。
  index 可选
    数组中正在处理的当前元素的索引。 如果提供了initialValue，则起始索引号为0，否则从索引1起始。
  array可选
   调用reduce()的数组
  initialValue可选
   作为第一次调用 callback函数时的第一个参数的值。 如果没有提供初始值，则将使用数组中的第一个元素。 在没有初始值的空数组上调用 reduce 将报错。

返回值：
函数累计处理的结果


练习完整代码如下所示：

function sumFibs(num) {
  if (num <= 0) return 0;

  const arrFib = [1, 1];
  let nextFib = 0;

  while ((nextFib = arrFib[0] + arrFib[1]) <= num) {
    arrFib.unshift(nextFib);
  }

  return arrFib.filter(x => x % 2 != 0).reduce((a, b) => a + b);
}

console.log( sumFibs(11) );
// => 10

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
