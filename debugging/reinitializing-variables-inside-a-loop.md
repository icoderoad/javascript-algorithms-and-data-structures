---
id: 6029b27d874868e70dce168f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 重新初始化循环中的变量时要小心
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/debuging.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

重新初始化循环中的变量时要小心

有时需要在循环中保存信息以增加计数器或重置变量。一个潜在的问题是变量什么时候该重新初始化，什么时候不该重新初始化，反之亦然。如果不小心重置了用于终止条件的变量，导致无限循环，这将特别危险。

使用 console.log() 在每个循环中打印变量值可以发现与重置相关的错误或者重置变量失败。

以下函数应该创建一个具有 m 行和 n 列“零”的二维数组。不幸的是，它没有产生预期的输出，因为 row 变量没有在外部循环中重新初始化（设置回空数组）。我们先在控制台执行以下代码，看下控制台输出结果。然后再修改代码，使其正确地返回包含 3 行 2 列“零”的二维数组，即[[0, 0], [0, 0], [0, 0]]。


function zeroArray(m, n) {
  let newArray = [];
  
  for (let i = 0; i < m; i++) {
  	let row = [];
    for (let j = 0; j < n; j++) {
      row.push(0);
    }
    newArray.push(row);
  }
  return newArray;
}

let matrix = zeroArray(3, 2);
console.log(matrix);

由于重新初始化循环中的变量有问题，执行以上代码，控制台输出 3 行 6 列代码，不是我们希望的 3 行 2 列效果。输出结果如下所示：

0: (6) [0, 0, 0, 0, 0, 0]
1: (6) [0, 0, 0, 0, 0, 0]
2: (6) [0, 0, 0, 0, 0, 0]

修改以上代码，我们只调整了下行数据初始化的位置，将行数组初始化代码 let row = []; 放在行循环内部，就可以实现我们想要的 m 行 n 列的效果。


function zeroArray(m, n) {
  let newArray = [];
  
  for (let i = 0; i < m; i++) {
  	let row = [];
    for (let j = 0; j < n; j++) {
      row.push(0);
    }
    newArray.push(row);
  }
  return newArray;
}

let matrix = zeroArray(3, 2);
console.log(matrix);

0: (2) [0, 0]
1: (2) [0, 0]
2: (2) [0, 0]

matrix = zeroArray(5, 6);
console.log(matrix);

(5) [Array(6), Array(6), Array(6), Array(6), Array(6)]
0: (6) [0, 0, 0, 0, 0, 0]
1: (6) [0, 0, 0, 0, 0, 0]
2: (6) [0, 0, 0, 0, 0, 0]
3: (6) [0, 0, 0, 0, 0, 0]
4: (6) [0, 0, 0, 0, 0, 0]

以上代码我们测试了 3 行 2 列和 5 行 6 列的输出效果，都按我们想要的方式正确输出。大家也可以换不同的行列数值，测试下最终的输出效果。

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
