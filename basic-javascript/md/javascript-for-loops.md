---
id: 5fe035eefb445251f8faa0ad
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: for 循环语句用法详解
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
for 循环语句用法详解。

今天我们介绍 JavaScript 语言中的第二种循环类型 for 循环，它是 JavaScript 语言中最常见的循环。

for 循环中的三个表达式用分号隔开。

语法示例如下所示：

for ([初始化]; [条件判断]; [计数器])

初始化语句只会在执行循环开始之前执行一次。它通常用于定义和设置循环变量。

条件判断语句会在每一轮循环的开始执行，只要条件判断为 true 就会继续执行循环。当条件为 false 的时候，循环将停止执行。这意味着，如果条件在一开始就为 false ，这个循环将不会执行。

计数器是在每一轮循环结束时执行，通常用于递增或递减。

我们继续以计算 1+2+3 ... +98+99+100 的值算法为例，通过 for 循环进行求值计算，代码如下所示：

var total =0;
for( var i=1; i<=100; i++) {
  total = total + i;
}

console.log( total ); // => 5050

在控制台执行上面代码后，会在控制台输出计算结果为 5050. 与 while 循环计算结果一致。

for 循环可以按照我们指定的顺序来迭代，通过更改我们的计数器，我们可以按照奇偶数顺序来迭代。

我们继续调整上面的代码，将计数器部分进行调整，i += 2 让 i 每次循环之后增加 2。计算 1 至 100 内的奇数之和，代码如下所示：

var total =0;
for( var i=1; i<=100; i += 2) {
  total = total + i;
}

console.log( total ); // => 2500

以上代码在控制台执行后，控制台打印输出结果为 2500，大家可以与前面讲解的 while 循环计算奇数的代码进行比较下，使用 for 循环代码更为简洁。

for 循环也可以逆向迭代，只要我们定义好合适的条件。我们继续调整上面代码，还是计算 100 以内所有奇数之和。为了让每次倒数递减 2，我们需要改变我们的初始化条件，条件判断和计数器。

我们让初始值为 i = 99，并且当 i > 0 的时候才继续循环。我们使用i  -= 2 来让 i 每次循环递减 2 。

var total =0;
for( var i=99; i>0 ; i -= 2) {
  total = total + i;
}

console.log( total ); // => 2500


迭代输出一个数组的每个元素是 JavaScript 语言中的常见需求，for 循环可以做到这一点。下面的代码将 1 至 100 内所有整数添加至数组 arr ,然后通过循环数组里的每个元素求和，计算 1+2+3 ... +98+99+100 的值，并将最终计算结果输出至控制台 ：

var arr = [];
for (var i = 1; i <=100 ; i++) {
   arr.push(i);
}
console.log(arr);
var total =0;
for( var i=0; i<arr.length; i++ ){
  total += arr[i];
}

console.log( total ); // => 5050

注意：数组的索引从零开始的，这意味着数组的最后一个元素的下标是：数组的长度 -1。我们这个循环的条件是 i < arr.length ，当 i 的值为长度 -1 的时候循环就停止了。

如果你有一个二维数组，可以使用相同的逻辑，先遍历外面的数组，再遍历里面的子数组。下面是一个例子：

var arr = [
  [1,2], [3,4], [5,6]
];

var total =0;
for (var i=0; i < arr.length; i++) {
  for (var j=0; j < arr[i].length; j++) {
    total += arr[i][j];
  }
}

console.log( total ); // => 21

控制台最后会输出每个子数组中每个元素的求和结果 21。

提示：对于内部循环，我们可以通过 arr[i].length 来获得子数组的长度，因为 arr[i] 的本身就是一个数组。

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
