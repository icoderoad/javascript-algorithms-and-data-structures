---
id: 608a44ac8c041f364b3a9da5
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 concat 方法将元素添加到数组的末尾
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组 reduce 方法分析数据

reduce()（即Array.prototype.reduce()），是 JavaScript 所有数组操作中最常用的方法。几乎可以用reduce方法解决所有数组处理问题。

reduce 方法是处理数组更通用的方式，而且 filter 和 map 方法都可以当作是 reduce 的特殊实现。 reduce  方法遍历数组中的每个项目并返回单个值（即字符串、数字、对象、数组）。 这是通过在每次迭代中调用一个回调函数来实现的。

在介绍具体示例之前，我们先介绍下 reduce() 方法的具体用法：

reduce() 方法对数组中的每个元素执行一个由您提供的reducer函数(升序执行)，将其结果汇总为单个返回值。

reduce()  方法接收4个参数:

Accumulator (acc) (累计器)
Current Value (cur) (当前值)
Current Index (idx) (当前索引)
Source Array (src) (源数组)

reduce() 方法的返回值分配给累计器，该返回值在数组的每个迭代中被记住，并最后成为最终的单个结果值。

语法:
  arr.reduce(callback(accumulator, currentValue[, index[, array]])[, initialValue])

参数:
  callback
    执行数组中每个值 (如果没有提供 initialValue 则第一个值除外)的函数，包含四个参数：

    accumulator
      累计器累计回调的返回值; 它是上一次调用回调时返回的累积值，或 initialValue（见于下方）。

    currentValue
      数组中正在处理的元素。

    index 可选
      数组中正在处理的当前元素的索引。 如果提供了 initialValue，则起始索引号为 0，否则从索引1起始。

    array可选
      调用 reduce() 的数组

  initialValue可选
    作为第一次调用 callback 函数时的第一个参数的值。 如果没有提供初始值，则将使用数组中的第一个元素。 在没有初始值的空数组上调用 reduce 将报错。

返回值:
  函数累计处理的结果


回调函数接受四个参数。第一个参数称为累计器，它是上一次迭代中回调函数的返回值，第二个参数是当前正在处理的数组元素，第三个参数是该参数的索引，第四个参数是在其上调用 reduce()  方法的数组。

除了回调函数，reduce()  还有一个额外的参数做为叠加器的初始值。如果没有第二个参数，会跳过第一次迭代，第二次迭代给累计器传入数组的第一个元素。

见下面的例子，给 sites 站点数组使用 reduce() 方法，返回所有网站员工数之和。为了简化，例子仅使用了回调函数的第一个参数和第二个参数。

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

const userTotal = sites.reduce((sum, site) => sum + site.userNum, 0);
console.log(userTotal); 
// => 12791

在下面的示例里，我们通过 reduce() 方法 对 sites 数组进行处理，返回一个包含网站名称做为属性，其员工数做为值的对象。

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

const sitesObj = sites.reduce((obj, site) => {
  obj[site.name] = site.userNum;
  return obj;
}, {});

console.log(sitesObj); 
// => {腾讯: 5200, 京东: 3210, 天猫: 4231, 路条编程: 150}


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
