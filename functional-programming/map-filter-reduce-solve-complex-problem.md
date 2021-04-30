---
id: 608b647751e01039f2a3adfc
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用方法 map、filter 或者 reduce 来解决复杂问题
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用方法 map、filter 或者 reduce 来解决复杂问题

前面文章中我们已经介绍过数组的常用方法，如 map()、 filter() 和 reduce()的使用，现在是时候用它们来完成一些复杂的问题的处理了。

今天我们通过一个完整的练习介绍下这几个常用方法来处理复杂的问题。我们定义一个方法 numberPowArr。方法包含一个参数 arr, 为要处理的数字数组，我们可以通过任意组合 map()、filter() 和 reduce() 方法来完成我们定义的方法，函数返回仅包含正整数的平方的新数组。

由于我们要练习 map()、filter() 和 reduce() 方法 的使用，我们实现的方法不能使用任何形式的 for 、 while 循环或者 forEach() 方法。

具体实现代码如下所示：

方法1:

const numberPowArr = (numArr) => {
  return numArr
          .filter(num => num > 0 && num % parseInt(num) === 0)
          .map(num => Math.pow(num, 2));
};

const numArrs = numberPowArr([-11, 8.8, 7, -13, 7.2, 15]);
console.log(numArrs);
// => (2) [49, 225]


方法2:

const numberPowArr2 = (numArr) => {
  return numArr.reduce((numArrs2, num) => {
    return Number.isInteger(num) && num > 0
      ? numArrs2.concat(num * num)
      : numArrs2;
  }, []);
};

const numArrs2 = numberPowArr2([-3.7, 51, -23, 40, 12.5, 7, -4.5, -17, 8]);
console.log(numArrs2);
// => (4) [2601, 1600, 49, 64]

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
