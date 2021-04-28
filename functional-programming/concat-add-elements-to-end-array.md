---
id: 6088f51b56b7610821bdb8f2
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 concat 方法将元素添加到数组的末尾
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用 concat 方法将元素添加到数组的末尾

函数式编程就是创建和使用具有不变性的函数。

上篇文章我们介绍了 concat 方法的基础用法，这是一种在不改变原始数组的前提下，将数组组合成新数组的方法。将 concat 方法与 push 方法做比较，push 方法将元素添加到调用它的数组的末尾，这样会改变该数组。举个例子：

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

const asites = [
  { name: '百度', domain: "www.baidu.com", userNum: 4000 }
];

sites.push( asites );
console.log(sites);
// => 0: {name: "腾讯", domain: "www.qq.com", userNum: 5200}
// => 1: {name: "京东", domain: "www.jd.com", userNum: 3210}
// => 2: {name: "天猫", domain: "www.tmall.com", userNum: 4231}
// => 3: {name: "路条编程", domain: "www.icoderoad.com", userNum: 150}
// => 4: Array(1)
// => 0: {name: "百度", domain: "www.baidu.com", userNum: 4000}
// => length: 1

下面我们练习一个完整的示例，先定义一个方法 concatArrSite, 包含两个参数 sites 和 nsites，通过 concat 方法将新站点数组 nsites 添加到站点数组 sites 末尾，该函数应返回一个合并后的站点新数组。原站点数组 sites 不产生任何变化。

function concatArrSite(sites, nsites) {
  return sites.concat(nsites);
}

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

const nsites = [
  { name: '百度', domain: "www.baidu.com", userNum: 4000 }
];

concatArrSite(sites, nsites)

console.log( sites );
// => 0: {name: "腾讯", domain: "www.qq.com", userNum: 5200}
// => 1: {name: "京东", domain: "www.jd.com", userNum: 3210}
// => 2: {name: "天猫", domain: "www.tmall.com", userNum: 4231}
// => 3: {name: "路条编程", domain: "www.icoderoad.com", userNum: 150}

通过执行以上代码可知，控制台打印输出原站点数组 sites 的值没有产生任何变化。


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
