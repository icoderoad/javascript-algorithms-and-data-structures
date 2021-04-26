---
id: 6086640e37f9527f8bdeb05c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组 slice 方法从数组中移除元素
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组 slice 方法从数组中移除元素

我们在实际工作过程中，经常遇到使用数组要删除一些元素并保留数组剩余部分的情况。为此，JavaScript 提供了 splice 方法，在介绍具体示例之前，先介绍下数组 slice 方法的具体用法。

slice 方法可以从已有数组中返回指定元素。它接受两个参数，第一个规定从何处开始选取，第二个规定从何处结束选取（不包括该元素）。如果没有传参，则默认为从数组的开头开始到结尾结束，这是复制整个数组的简单方式。slice 返回一个新数组，不会修改原始数组。

语法：
arr.slice([begin[, end]])

参数：
  begin 可选
    提取起始处的索引（从 0 开始），从该索引开始提取原数组元素。

    如果该参数为负数，则表示从原数组中的倒数第几个元素开始提取，slice(-2) 表示提取原数组中的倒数第二个元素到最后一个元素（包含最后一个元素）。
    如果省略 begin，则 slice 从索引 0 开始。

    如果 begin 超出原数组的索引范围，则会返回空数组。
  end 可选
    提取终止处的索引（从 0 开始），在该索引处结束提取原数组元素。slice 会提取原数组中索引从 begin 到 end 的所有元素（包含 begin，但不包含 end）。

    slice(1,4) 会提取原数组中从第二个元素开始一直到第四个元素的所有元素 （索引为 1, 2, 3的元素）。

    如果该参数为负数， 则它表示在原数组中的倒数第几个元素结束抽取。 slice(-2,-1) 表示抽取了原数组中的倒数第二个元素到最后一个元素（不包含最后一个元素，也就是只有倒数第二个元素）。

    如果 end 被省略，则 slice 会一直提取到原数组末尾。

    如果 end 大于数组的长度，slice 也会一直提取到原数组末尾。

返回值：
  一个含有被提取元素的新数组。

正如我们在上篇文章中看到的那样，slice 方法不会改变原始数组，而是返回一个可以保存到变量中的新数组。回想一下，slice 方法接收两个参数，从开始索引开始选取到结束（不包括该元素），并在新数组中返回这些元素。使用 slice 方法替代 splice 有助于避免数组变化产生的副作用。

我们定义一个函数 sliceArr3Ele， 该方法接收一个数组参数 sites, 返回站点数组的前 3 项元素的的新数组。

具体示例代码如下所示：

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

function sliceArr3Ele(sites) {

  return sites.slice(0, 3);

}
console.log( sliceArr3Ele( sites ) );
// => 0: {name: "腾讯", domain: "www.qq.com", userNum: 5200}
// => 1: {name: "京东", domain: "www.jd.com", userNum: 3210}
// => 2: {name: "天猫", domain: "www.tmall.com", userNum: 4231}

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
