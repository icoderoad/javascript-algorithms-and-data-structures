---
id: 60a0cd91ed86e04a947f6608
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将传入字符串中每个字符获取与其配对的元素返回
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

将传入字符串中每个字符获取与其配对的元素返回

本次练习我们需要写一个函数 strPairElement 。该方法接收一个参数 str，该方法把传入的字符串中每个字符，获取与其配对的元素，并将结果作为二维数组返回。

碱基对是一对 AT 和 CG。将缺少的元素与提供的字符匹配。

将提供的字符作为每个数组中的第一个元素返回。

例如，对于输入 GCG，返回[[“G”, “C”]，[“C”, “G”]，[“G”, “C”]]。

字符及与其配对的元素在一个数组中。再将所有数组放到一个封装数组中。


在介绍完整代码之前，我们先介绍下数组 map 方法的具体用法： 

map() 方法创建一个新数组，其结果是该数组中的每个元素是调用一次提供的函数后的返回值。

语法：
var new_array = arr.map(function callback(currentValue[, index[, array]]) {
 // Return element for new_array 
}[, thisArg])

参数：
  callback
    生成新数组元素的函数，使用三个参数：
    currentValue
      callback 数组中正在处理的当前元素。
    index可选
      callback 数组中正在处理的当前元素的索引。
    array可选
      map 方法调用的数组。
  thisArg可选
    执行 callback 函数时值被用作this。

返回值：
一个由原数组每个元素执行回调函数的结果组成的新数组。

练习完整代码如下所示：

function strPairElement( str ){
  var pairs = {
    A: "T",
    T: "A",
    C: "G",
    G: "C"
  };
  var arr = str.split("");
  return arr.map(x => [x, pairs[x]]);
}

console.log( strPairElement('GTCAGT') );
// => 0: (2) ["G", "C"]
// => 1: (2) ["T", "A"]
// => 2: (2) ["C", "G"]
// => 3: (2) ["A", "T"]
// => 4: (2) ["G", "C"]
// => 5: (2) ["T", "A"]

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
