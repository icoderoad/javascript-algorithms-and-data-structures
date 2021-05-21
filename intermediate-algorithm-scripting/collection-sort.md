---
id: 60a350ee35b0df4e0ac72229
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将多个数组中所有元素进行去除重复元素排序返回
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

将多个数组中所有元素进行去除重复元素排序返回

本次练习我们需要写一个函数 collectionSort 。该方法接收两个或多个数组为参数，该方法找需要对这些数组中所有元素进行去除重复元素的处理，并以数组的形式返回去重结果。

换句话说，所有数组中出现的所有值都应按其原始顺序包括在内，但最终数组中不得重复。

唯一数字应按其原始顺序排序，但最终数组不应按数字顺序排序。


在介绍完整代码之前，我们先介绍下arguments 对象的具体用法： 

arguments 是一个对应于传递给函数的参数的类数组对象。

arguments对象是所有（非箭头）函数中都可用的局部变量。你可以使用 arguments 对象在函数中引用函数的参数。此对象包含传递给函数的每个参数，第一个参数在索引0处。

arguments 对象不是一个 Array 。它类似于 Array，但除了 length 属性和索引元素之外没有任何 Array 属性。

如果调用的参数多于正式声明接受的参数，则可以使用 arguments 对象。这种技术对于可以传递可变数量的参数的函数很有用。使用 arguments.length 来确定传递给函数参数的个数，然后使用 arguments 对象来处理每个参数。

练习完整代码如下所示：

function collectionSort(){
  var newArr;
  var args = Array.prototype.slice.call(arguments);
  newArr = args.reduce(function(arrA, arrB) {
    return arrA.concat(
      arrB.filter(function(i) {
        return arrA.indexOf(i) === -1;
      })
    );
  });

  return newArr;
}

console.log( collectionSort([51, 32, 13], [75, 2, 81, 32], [11, 63], [63, 32, 41]) );
// => (9) [51, 32, 13, 75, 2, 81, 11, 63, 41]

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
