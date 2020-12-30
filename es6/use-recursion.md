---
id: 5fe96f721d81c96c16b14d5b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用递归创建一个倒计时和数字序列实例
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用递归创建一个倒计时和数字序列实例。

前面的文章中我们介绍了怎样用递归来代替循环。现在来学习两个更复杂的递归函数作为本章的结尾。
第一个是倒计时函数，函数返回一个从 1 到传递给函数的指定数字的连续数字数组。

正如前面文章介绍的，会有一个基本条件。基本条件告诉递归函数什么时候不在需要调用其自身。这是简单情况，返回得到的值。还有递归调用条件，继续用不同的参数调用自身。如果函数无误，一直执行直到基本条件为止。

比如，如果想写一个递归函数，返回一个数字 1 到 n 的连续数组。这个函数需要接收一个参数 n 代表起始数字。然后会持续的调用自身，传入一个比 n 更小的值一直到传入的值是 1 为止。函数如下：

function countup(n) {
  if (n < 1) {
    return [];
  } else {
    const countArray = countup(n - 1);
    countArray.push(n);
    return countArray;
  }
}
console.log(countup(5)); // => [ 1, 2, 3, 4, 5 ]

起初，这似乎是违反直觉的，因为 n 的值递减，但是最终数组中的值却递增。 之所以发生这种情况，是因为在递归调用返回之后，才调用 push。 在将 n countup(n - 1) 已经调用赋值成功并返回了 [1, 2, ..., n - 1]。


现在我们定义了一个类似倒计时的函数 countdown，函数有一个参数（n）。函数应该基于参数 n 递归调用返回 n 到 1 的连续数字的数组。如果函数以小于 1 的参数调用，函数应该返回空数组。 比如，用 n = 5 调用函数应该返回数组 [5, 4, 3, 2, 1]。 函数必需使用递归函数调用自身，不能使用任何形式的循环。

function countdown(n) {
  if (n < 1) {
    return [];
  } else {
    const arr = countdown(n - 1);
    arr.unshift(n);
    return arr;
  }
}

上面代码示例使用了 unshift() 方法， unshift() 方法将一个或多个元素添加到数组的开头，并返回该数组的新长度(该方法修改原有数组)。

下面我们定义一个 rangeOfNumbers 函数，包含两个参数。函数应该返回一个连续数字数组，startNum 参数表示开始数字， endNum 参数表示截止数字。开始的数字小于或等于截止数字。函数必需递归调用自身，不能使用任意形式的循环。要考虑到参数 startNum 和 endNum 相同的情况。

function rangeOfNumbers(startNum, endNum) {
  if (endNum - startNum === 0) {
    return [startNum];
  } else {
    var numbers = rangeOfNumbers(startNum, endNum - 1);
    numbers.push(endNum);
    return numbers;
  }
}

console.log( rangeOfNumbers(1, 4) ); // => [1, 2, 3, 4]
console.log( rangeOfNumbers(6, 9) ); // => [6, 7, 8, 9]
console.log( rangeOfNumbers(8, 8) ); // => [8]

到今天为止，我们 JavaScript 基础部分的内容就讲完了，下面我们继续学习 ES6 专题相关的知识。感兴趣的同学请继续关注公众号，每天准时发送。
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
