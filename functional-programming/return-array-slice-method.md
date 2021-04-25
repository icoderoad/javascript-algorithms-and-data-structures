---
id: 608519a719c11395ec2efa73
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组 slice 方法返回数组的一部分元素
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组 slice 方法返回数组的一部分元素

在介绍具体示例之前，我们先介绍下 Array.prototype.slice() 方法的具体用法：

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


举个例子：

function sliceSite(sites, begin, end) {
  
  return sites.slice(begin, end);

}

const sites = [
  { name: '腾讯', domain: "www.qq.com", userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

var mSites = sliceSite(sites, 1, 2);
console.log( mSites );
// =>  0: {name: "京东", domain: "www.jd.com", userNum: 3210}

以上代码定义了一个提取站点的方法 sliceSite，此方法有三个参数 sites、 begin 和 end，通过 begin 和 end 参数对 sites 数组进行数据提取。将提取的新数组赋值给变量 mSites，并将结果打印至控制台输出。

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
