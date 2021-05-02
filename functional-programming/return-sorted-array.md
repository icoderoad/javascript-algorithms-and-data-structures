---
id: 608e092a1839b7017eea3db8
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 返回排序后不更改原始数据数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

返回排序后不更改原始数据数组

上篇文章介绍的数组 sort() 方法会产生改变原始数组中元素顺序的副作用。换句话说，它会改变数组的位置。避免这种情况的一种方法是先将空数组连接到正在排序的数组上

记住通过使用 concat 方法返回一个新数组，再用 sort 方法。

在详解具体实例之前，我们再熟悉下 concat() 方法的具体用法。

concat() 方法用于合并两个或多个数组。此方法不会更改现有数组，而是返回一个新数组。

语法：
var new_array = old_array.concat(value1[, value2[, ...[, valueN]]])

参数：
  valueN 可选，数组和/或值，将被合并到一个新的数组中。如果省略了所有 valueN 参数，则 concat 会返回调用此方法的现存数组的一个浅拷贝。详情请参阅下文描述。

返回值：
新的 Array 实例。

描述：
concat 方法创建一个新的数组，它由被调用的对象中的元素组成，每个参数的顺序依次是该参数的元素（如果参数是数组）或参数本身（如果参数不是数组）。它不会递归到嵌套数组参数中。

concat 方法不会改变this或任何作为参数提供的数组，而是返回一个浅拷贝，它包含与原始数组相结合的相同元素的副本。



在 nonChangeeSiteSort 函数中使用 sort 方法对数组中的元素按升序进行排列。函数不能改变 sties 变量，应返回一个新数组。

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

function nonChangeeSiteSort(arr) {
  return [].concat(arr).sort(function(sitea, siteb) {
    return sitea.userNum - siteb.userNum;
  });
}

console.log(nonChangeeSiteSort(sites));
// => 0: {name: "路条编程", domain: "www.icoderoad.com", userNum: 150}
// => 1: {name: "京东", domain: "www.jd.com", userNum: 3210}
// => 2: {name: "天猫", domain: "www.tmall.com", userNum: 4231}
// => 3: {name: "腾讯", domain: "www.qq.com", userNum: 5200}

console.log(sites);
// => 0: {name: "腾讯", domain: "www.qq.com", userNum: 5200}
// => 1: {name: "京东", domain: "www.jd.com", userNum: 3210}
// => 2: {name: "天猫", domain: "www.tmall.com", userNum: 4231}
// => 3: {name: "路条编程", domain: "www.icoderoad.com", userNum: 150}

经过上面示例代码输出可知，方法 nonChangeeSiteSort 对网站数组 sites 中网站员工数按升序进行排列，调用方法 nonChangeeSiteSort 后，未改变 sites 数组中元素顺序。

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
