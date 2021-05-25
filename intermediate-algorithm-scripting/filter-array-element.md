---
id: 60a83a8be9d4771ecacc0778
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 筛选出数组中满足条件的元素

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

筛选出数组中满足条件的元素

本次练习我们需要写一个函数 filterArrayElement ，它接收两个参数 arr, func，它的返回由原数组中第一个使得func为true的元素及其之后的所有元素组成的数组。

给定数组 arr，从数组的第一个元素开始，用函数 func 来检查数组的每个元素并删除，直到某个元素传入函数func时返回true。

如果数组中的所有元素都不能让 func为true，则返回空数组[]。

在介绍完整代码之前，我们先介绍下数组 slice 方法的具体用法： 

slice() 方法返回一个新的数组对象，这一对象是一个由 begin 和 end 决定的原数组的浅拷贝（包括 begin，不包括end）。原始数组不会被改变。

语法:
arr.slice([begin[, end]])

参数:
  begin 可选
    提取起始处的索引（从 0 开始），从该索引开始提取原数组元素。
    如果该参数为负数，则表示从原数组中的倒数第几个元素开始提取，slice(-2) 表示提取原数组中的倒数第二个元素到最后一个元素（包含最后一个元素）。
    如果省略 begin，则 slice 从索引 0 开始。
    如果 begin 超出原数组的索引范围，则会返回空数组。
  end 可选
    提取终止处的索引（从 0 开始），在该索引处结束提取原数组元素。slice 会提取原数组中索引从 begin 到 end 的所有元素（包含 begin，但不包含 end）。
    slice(1,4) 会提取原数组中从第二个元素开始一直到第四个元素的所有元素 （索引为 1, 2, 3的元素）。
    如果该参数为负数， 则它表示在原数组中的倒数第几个元素结束抽取。 slice(-2,-1) 表示抽取了原数组中的倒数第二个元素到最后一个元素（不包含最后一个元素，也就是只有倒数第二个元素）。
    如果 end 被省略，则 slice 会一直提取到原数组末尾。
    如果 end 大于数组的长度，slice 也会一直提取到原数组末尾。

返回值:
一个含有被提取元素的新数组。

练习完整代码如下所示：

function filterArrayElement(arr, func) {
   let sliceIndex = arr.findIndex(func);
   return arr.slice(sliceIndex >= 0 ? sliceIndex : arr.length);
}

console.log( filterArrayElement([1, 2, 3, 4], function(n) {return n > 5;}) );
// => []

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
