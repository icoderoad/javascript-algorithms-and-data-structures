---
id: 60ac8e7858bf91ecfc484e21
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 创建一个将两个参数相加的函数

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

创建一个将两个参数相加的函数

本次练习我们需要写一个函数 addNumber ，它接收一个或两个参数，如果只传入了一个参数，则返回一个函数，需要传入一个参数并返回总和。

addNumber(2, 3)应该返回 5。而 addNumber(2)应该返回一个函数。

调用这个返回的函数，传入一个值，返回总和：

var sumTwoAnd = aaddNumber(3);

addNumber(3) 此时应返回6。

只要其中任何一个参数不是数字，那就应返回 undefined。

在介绍完整代码之前，我们先介绍下 Object.values() 方法的具体用法： 

Object.values()方法返回一个给定对象自身的所有可枚举属性值的数组，值的顺序与使用 for...in 循环的顺序相同 ( 区别在于 for-in 循环枚举原型链中的属性 )。

语法：
Object.values(obj)

参数：
obj
被返回可枚举属性值的对象。

返回值：
一个包含对象自身的所有可枚举属性值的数组。

练习完整代码如下所示：

function addNumber() {
   const [first, second] = Object.values(arguments);
  //检查第一个参数是否为数字
  if (typeof first !== "number") {
    return undefined;
  }

  // 添加第2个参数
  const addSecond = (second) => typeof second === "number" ? first + second : undefined;

  // 检查是否为两个合法的数字参数
  if (second !== undefined) {
    return addSecond(second);
  } else {
    return addSecond
  }
}

console.log( addTogether(4, 6));
// => 10

console.log( addTogether("www.icoderoad.com"));
// => undefined

console.log( addTogether(2, "3"));
// => undefined

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
