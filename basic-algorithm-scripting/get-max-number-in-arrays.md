---
id: 6049adacc3158e6605a55747
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 获取二维数组中的子数组的最大数数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

获取二维数组中的子数组的最大数数组

今天我们做个获取数组中最大数字数组的练习。我们使用数组的 map 方法和 for 循环来遍历数组。我们使用一个二维数组进行演示，该数组每个元素由不定数量数字子数组组成。在做练习之前，我们先介绍下数组 map 方法。

map() 方法创建一个新数组，其结果是该数组中的每个元素是调用一次提供的函数后的返回值。

语法：

var new_array = arr.map(function callback(currentValue[, index[, array]]) {
 // 返回新数组
}[, thisArg])

参数：

callback	生成新数组元素的函数，使用三个参数：

currentValue	callback 数组中正在处理的当前元素。

index	可选，callback 数组中正在处理的当前元素的索引。

array 可选，map 方法调用的数组。

thisArg	可选，执行 callback 函数时值被用作 this。

返回值：

一个由原数组每个元素执行回调函数的结果组成的新数组。

为了实现我们的要求，我们需要定义一个方法 getlargestNumInArrs 参数为 arrs，为我们要查找的二维数组，该方法的返回值为所有子数组中最大的一个数字。具体实现步骤如下所示：

1、调用数组 map 方法遍历二维数组

2、获取子数组第一个元素赋值给一个临时变量

3、循环子数组中的每个元素，也临时变量比较，如果当前元素大于临时变量，使用当前值替换临时变量值

4、返回临时变量

具体实现代码如下所示：


function getlargestNumInArrs( arrs ) {
  let result = arrs.map(item => {
    let temp = item[0]
    for(let i = 0;i < item.length;i++) {
      temp > item[i] ? '' : temp = item[i]
    }
    return temp
  })
  return result;
}
 
let mArrs = getlargestNumInArrs([[3, 13, 1, 7, 21], [23, 42, 11], [103, 21], [90101, 1103, 857, 1, 99]]);
console.log( mArrs );
// => (4) [21, 42, 103, 90101]

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
