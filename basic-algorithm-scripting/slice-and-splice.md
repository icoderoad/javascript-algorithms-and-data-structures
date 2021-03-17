---
id: 6051a6bdfc981994c749db38
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组方法 slice 和 splice 方法按顺序将第一个数组的每个元素复制到第二个数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用数组方法 slice 和 splice 方法按顺序将第一个数组的每个元素复制到第二个数组

今天我们介绍数组之间操作的问题。此方法有三个参数，三个参数分别为 arr1、arr2 和 n 。使用数组方法 slice 和 splice 按顺序将第一个数组的每个元素复制到第二个数组中。在第二个数组的索引 n 处插入复制的第一个数组元素。返回合并后的数组数据。方法运行后，输入数组应保持不变。在介绍具体方法之前，我们先介绍下数组的 slice() 方法和 splice() 方法。

slice() 方法返回一个新的数组对象，这一对象是一个由 begin 和 end 决定的原数组的浅拷贝（包括 begin，不包括end）。原始数组不会被改变。

语法：

arr.slice([begin[, end]])

参数：

begin 可选，提取起始处的索引（从 0 开始），从该索引开始提取原数组元素。

如果该参数为负数，则表示从原数组中的倒数第几个元素开始提取，slice(-2) 表示提取原数组中的倒数第二个元素到最后一个元素（包含最后一个元素）。

如果省略 begin，则 slice 从索引 0 开始。

如果 begin 超出原数组的索引范围，则会返回空数组。

end 可选，提取终止处的索引（从 0 开始），在该索引处结束提取原数组元素。slice 会提取原数组中索引从 begin 到 end 的所有元素（包含 begin，但不包含 end）。

slice(1,4) 会提取原数组中从第二个元素开始一直到第四个元素的所有元素 （索引为 1, 2, 3的元素）。

如果该参数为负数， 则它表示在原数组中的倒数第几个元素结束抽取。 slice(-2,-1) 

表示抽取了原数组中的倒数第二个元素到最后一个元素（不包含最后一个元素，也就是只有倒数第二个元素）。

如果 end 被省略，则 slice 会一直提取到原数组末尾。

如果 end 大于数组的长度，slice 也会一直提取到原数组末尾。

返回值：

一个含有被提取元素的新数组。


splice() 方法通过删除或替换现有元素或者原地添加新的元素来修改数组,并以数组形式返回被修改的内容。此方法会改变原数组。

语法：

array.splice(start[, deleteCount[, item1[, item2[, ...]]]])

参数：

start​ 	指定修改的开始位置（从0计数）。如果超出了数组的长度，则从数组末尾开始添加内容；如果是负值，则表示从数组末位开始的第几位（从-1计数，这意味着-n是倒数第n个元素并且等价于array.length-n）；如果负数的绝对值大于数组的长度，则表示开始位置为第0位。

deleteCount 可选，整数，表示要移除的数组元素的个数。如果 deleteCount 大于 start 之后的元素的总数，则从 start 后面的元素都将被删除（含第 start 位）。

如果 deleteCount 被省略了，或者它的值大于等于array.length - start(也就是说，如果它大于或者等于start之后的所有元素的数量)，那么start之后数组的所有元素都会被删除。

如果 deleteCount 是 0 或者负数，则不移除元素。这种情况下，至少应添加一个新元素。

item1, item2, ... 可选，要添加进数组的元素,从start 位置开始。如果不指定，则 splice() 将只删除数组元素。

返回值：

由被删除的元素组成的一个数组。如果只删除了一个元素，则返回只包含一个元素的数组。如果没有删除元素，则返回空数组。


算法实现步骤如下所示：

1、创建 arr2 的副本。

2、使用f循环进行数组遍历，从索引 n 开始将数组 arr1 每个元素插入到数组 arr2 

3、每次循环运行时，将 n 递增加 1


4、返回组合后的数组


function arrSplice(arr1, arr2, n) {
 
  let combinedArrays = arr2.slice()
  
  for (let i = 0; i < arr1.length; i++) {
      combinedArrays.splice(n, 0, arr1[i])
      n++
  }
  
  return combinedArrays
}

let mArr = arrSplice(["菜鸟", "008"], ["您好", "欢迎", "访问", "路条编程网站!"], 1) ;

console.log( mArr.join(''));

// => 您好菜鸟008欢迎访问路条编程网站!



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
