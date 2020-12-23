---
id: 5fe2d54ac1b86e800e1b21cf
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用递归代替循环
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用递归代替循环。

函数直接或间接调用自身的编程技巧称为递归。使用递归函数一定要注意，处理不当就会进入死循环。

为了便于理解，有如下任务：计算数组内元素第 0 到第 n 的元素乘积，使用 for 循环， 可以这样做：

function multiply(arr, n) {
    var num = arr[0];
    for (var i = 1; i <= n; i++) {
        num *= arr[i];
    }
    return num;
}


下面是递归写法，注意代码里的 multiply2(arr, n) == multiply2(arr, n - 1) * arr[n] 这条判断语句。这意味着可以重写 multiply2 以调用自身而无需依赖循环。

  function multiply2(arr, n) {
    if (n <= 0) {
      return arr[0];
    } else {
      return multiply2(arr, n - 1) * arr[n];
    }
  }

递归版本的 multiply2 详述如下。在最终遍历结束时，也就是 n <= 0 时，返回结果，也就是 arr[0]。在 n 比 0 大的情况里，函数会调用自身，参数 n 的值为 n - 1。函数以相同的方式持续调用 multiply2，直到 n = 0 为止。所以，所有函数都可以返回，原始的 multiply2 返回结果。

注意： 递归函数在没有函数调用时（在这个例子是，是当 n <= 0 时）必需有一个跳出结构，否则永远不会执行完毕。

下面我们给数组添加 10 个元素 ，数值分别为 1-10， 我们比较下两种方式实现的结果是否一致，代码如下所示：

var numArr = [];
for( var i=1;i <=10; i++ ){
	numArr.push(i);
}

console.log( multiply(numArr, numArr.length -1 ) );  // => 3628800
console.log( multiply2(numArr, numArr.length -1 ) ); // => 3628800


经过以上代码测试函数 multiply 和 multiply2 返回的结果相同。注意：因为数组的索引是从 0 开始，上面调用两函数时，参数 n 的值应为数组长度 -1 。

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
