---
id: 60470673f08c79c4374d522c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 整数的阶乘方法实现
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

整数的阶乘方法实现

今天我们通过两种方式实现整数阶乘的方法。 返回提供的整数的阶乘。如果整数用 n 表示，则阶乘是所有小于或等于 n 的正整数的乘积。因子通常用简写符号 n! 表示 n! 。
例如： 5! = 5 * 4 * 3 * 2 * 1 = 120 只有大于或等于零的整数才会被提供给该函数。

方法1: 递归实现
let i = 0;
let arr = [];
function fac(num) {
  i++;
  arr.push(num);
  console.log( '第' + i + ' 次迭代，num 值为：' + num);
 return num >1 ? num * fac(num-1):1;
}

console.log(" 递归方法实现整数阶乘，结果值为： ",fac(5) );
console.log(" 递归方法最终实现 5!=" + arr.join(" * ") );

第1 次迭代，num 值为：5
第2 次迭代，num 值为：4
第3 次迭代，num 值为：3
第4 次迭代，num 值为：2
第5 次迭代，num 值为：1
递归方法实现整数阶乘，结果值为：120

递归方法最终实现 5!=5 * 4 * 3 * 2 * 1

方法2: for 循环方式实现

let index = 0;
let arr = [];
function fac2(num){
    arr.push(num);
    for(var i= num-1; i>= 1; i--){
        index++;
        console.log( '第' + index + ' 次迭代，i 值为：' + i);
        arr.push(i);
        num *=i;
    }
   
    return num;
}

let val = fac2(5);

console.log(" for 循环方法实现整数阶乘，结果值为： ",val );
console.log(" for 循环方法最终实现 5!=" + arr.join(" * ") );

第1 次迭代，i 值为：4
第2 次迭代，i 值为：3
第3 次迭代，i 值为：2
第4 次迭代，i 值为：1
for 循环方法实现整数阶乘，结果值为：120
for 循环方法最终实现 5!=5 * 4 * 3 * 2 * 1



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
