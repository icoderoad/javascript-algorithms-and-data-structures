---
id: 5fde9da51232170a98443cf2
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: while 循环语句用法详解
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
while 循环语句用法详解。

今天我们介绍 JavaScript 语言中的第一种循环类型 while 循环，因为它规定，当 while 条件为真时，循环体内的代码块才会执行，反之不执行。

使用 break 语句终止当前循环，并使用 continue 语句跳过循环中的值。

语法示例如下所示：

while (condition) {
//执行代码块
}

参数说明：

condition 为在每次遍历循环之前求值的表达式。如果该条件的计算结果为 true，则执行代码块。当条件的计算结果为 false 时，执行代码将在 while 循环之后继续。    如果条件始终为真，则循环将永不结束。这种情况将使您的浏览器崩溃，切记切记。

要计算 1+2+3 ... +98+99+100 的值，我们常规的做法是通过变量设置初始值，执行多次相加操作，直到增加至 100 为止。类似下面的代码：

var total =0;
total = total + 1;
total = total + 2;
total = total + 3;
...
total = total + 100;

以上代码会重复多次，太麻烦了，通过 while 循环几行代码，可以方便的实现相同的效果，while 循环代码示例如下所示：

var total =0;
var i=1;
while ( i<=100 ) {
  total = total + i;
  i++;
}

console.log( total ); // => 5050

在上面的代码里，while 循环执行 100 次，每次循环把变量 i 的值与 total 变量相加后的结果赋值至变量 total ,最后在控制台将计算结果输出， total 最终的结果值为 5050 。

如果我们只想计算 1 至 100 内奇数的和，应该如何实现呢？我们可以在代码块内通过取模运算判断是否为奇偶数，然后通过 continue 语句跳过偶数，只计算奇数，代码实现如下所示：

var total =0;
var i=1;
while ( i<=100 ) {
  if( i % 2 == 0 ){
    i++;
    continue;
  }
  console.log('i=' + i );
  total += i;
  i++;
}

console.log( total ); // => 2500

以上代码执行后会在控制台输出以下信息：

i=1
i=3
i=5
...
i=95
i=97
i=99
2500

最终计算 1 至 100 内奇数之和为 2500。

在上面示例中，在我们不改变循环条件的情况下，如何计算 50 内偶数之和呢？我们可以通过 continue  + break 语句结合的方式实现相应的计算。代码示例如下所示：

var total =0;
var i=1;
while ( i<=100 ) {
  if( i % 2 == 1 ){
    i++;
    continue;
  }
  if( i>50 ){
    break;
  }
  console.log('i=' + i );
  total += i;
  i++;
}

console.log( total ); // => 650

以上代码执行后会在控制台输出以下信息：

i=2
i=4
i=6
...
i=46
i=48
i=50
650

注意：如果要使用带有条件( condition )的变量，请在循环之前对其进行初始化，然后在循环体内对其进行递增。如果忘记增加变量，循环将永远不会结束。

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
