---
id: 6087a26f144773f038e924be
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组 concat 方法组合两个数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组 concat 方法组合两个数组

Concatenation 意思是将元素连接到尾部。同理，JavaScript 为字符串和数组提供了 concat 方法。对数组来说，在一个数组上调用 concat 方法，然后提供另一个数组作为参数添加到第一个数组末尾，返回一个新数组，不会改变任何一个原始数组。在介绍具体示例前，我们介绍下数组 concat 方法的用法。

concat 方法创建一个新的数组，它由被调用的对象中的元素组成，每个参数的顺序依次是该参数的元素（如果参数是数组）或参数本身（如果参数不是数组）。它不会递归到嵌套数组参数中。

concat 方法不会改变 this 或任何作为参数提供的数组，而是返回一个浅拷贝，它包含与原始数组相结合的相同元素的副本。 原始数组的元素将复制到新数组中，如下所示：

对象引用（而不是实际对象）：concat 将对象引用复制到新数组中。 原始数组和新数组都引用相同的对象。 

也就是说，如果引用的对象被修改，则更改对于新数组和原始数组都是可见的。 这包括也是数组的数组参数的元素。

数据类型如字符串，数字和布尔（不是String，Number 和 Boolean 对象）：concat将字符串和数字的值复制到新数组中。

语法：
var new_array = old_array.concat(value1[, value2[, ...[, valueN]]])

参数：
valueN 可选，数组和/或值，将被合并到一个新的数组中。如果省略了所有 valueN 参数，则 concat 会返回调用此方法的现存数组的一个浅拷贝。

返回值：
新的 Array 实例

我们实现一个站点拼接的方法 concatSite，此方法有两个参数 sites, aSites。 在不改变原数组 sites 及添加数组 aSites 的情况下，返回拼接后的数组给变量 tSites，将变量在控制台打印输出。将完整示例代码如下所示：

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

const asites = [
  { name: '百度', domain: "www.baidu.com", userNum: 4000 },
  { name: '网易', domain: 'www.163.com', userNum: 2110},
  { name: '新浪', domain: 'www.sina.com.cn', userNum: 3121}
];

function concatSite(sites, aSites) {
  return sites.concat( aSites );
}

var tSites = concatSite(sites, asites);

console.log( tSites );
// => 0: {name: "腾讯", domain: "www.qq.com", userNum: 5200}
// => 1: {name: "京东", domain: "www.jd.com", userNum: 3210}
// => 2: {name: "天猫", domain: "www.tmall.com", userNum: 4231}
// => 3: {name: "路条编程", domain: "www.icoderoad.com", userNum: 150}
// => 4: {name: "百度", domain: "www.baidu.com", userNum: 4000}
// => 5: {name: "网易", domain: "www.163.com", userNum: 2110}
// => 6: {name: "新浪", domain: "www.sina.com.cn", userNum: 3121}


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
