---
id: 609a16bbfa16f2d21a3a178a
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 从初始数组中移除所有与后续参数相等的元素
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

从初始数组中移除所有与后续参数相等的元素

本次练习我们需要写一个函数 delSameEleFromArr 。传给它的第一个参数 arr 是数组，我们称他为初始数组。后续的参数数量是不确定的，可能有一个或多个。该方法需要实现的功能是，从初始数组中移除所有与后续参数相等的元素，并返回移除元素后的数组。

注意：可以使用 arguments 对象，也可以使用 ...，即“剩余参数”（Rest Parameters）语法。

在介绍完整代码之前，我们先介绍下数组 Object.values() 方法的具体用法： 

Object.values() 方法返回一个给定对象自身的所有可枚举属性值的数组，值的顺序与使用 for...in 循环的顺序相同 ( 区别在于 for-in 循环枚举原型链中的属性 )。

语法：
Object.values(obj)

参数：obj  被返回可枚举属性值的对象。

返回值：
一个包含对象自身的所有可枚举属性值的数组。

Object.values()返回一个数组，其元素是在对象上找到的可枚举属性值。属性的顺序与通过手动循环对象的属性值所给出的顺序相同。

练习完整代码如下所示：

function delSameEleFromArr( arr ){
  let valsToRemove = Object.values(arguments).slice(1);

  for (let i = 0; i < arr.length; i++) {
    for (let j = 0; j < valsToRemove.length; j++) {
      if (arr[i] === valsToRemove[j]) {
        delete arr[i];
      }
    }
  }
  return arr.filter(item => item !== null);
}

console.log( delSameEleFromArr(['路条编程', '阿里巴巴', '拼多多', '亚马逊'],'京东', '美团', '拼多多', '头条', '亚马逊') );
// => (2) ["路条编程", "阿里巴巴"]

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
