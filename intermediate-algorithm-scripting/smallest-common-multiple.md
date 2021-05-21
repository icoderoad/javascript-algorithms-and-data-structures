---
id: 60a83a8be9d4771ecacc0778
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 计算一个包含两个数字的数组两个数字范围内所有数字的最小公倍数

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

计算一个包含两个数字的数组两个数字范围内所有数字的最小公倍数

本次练习我们需要写一个函数 smallestNum ，它接收一个包含两个数字的数组 arr，它的返回值为这两个数字范围内所有数字（包含这两个数字）的最小公倍数。

注意：较小数不一定总是出现在数组的第一个元素。

两个或多个整数公有的倍数叫做它们的公倍数，其中除0以外最小的一个公倍数就叫做这几个整数的最小公倍数。

比如，传入[1, 3]，那么函数的返回结果应为 1、2、3 的最小公倍数，即为 6。

在介绍完整代码之前，我们先介绍下数组 sort 方法的具体用法： 

sort() 方法用原地算法对数组的元素进行排序，并返回数组。默认排序顺序是在将元素转换为字符串，然后比较它们的UTF-16代码单元值序列时构建的

语法:
arr.sort([compareFunction])

参数:
  compareFunction 可选
    用来指定按某种顺序进行排列的函数。如果省略，元素按照转换为的字符串的各个字符的Unicode位点进行排序。
    firstEl
    第一个用于比较的元素。
    secondEl
    第二个用于比较的元素。

返回值:
排序后的数组。请注意，数组已原地排序，并且不进行复制。

练习完整代码如下所示：

function smallestNum(arr) {
  const [min, max] = arr.sort((a, b) => a - b);
  const range = Array(max - min + 1)
    .fill(0)
    .map((_, i) => i + min);
  
  const upperBound = range.reduce((prod, curr) => prod * curr);
 
  for (let multiple = max; multiple <= upperBound; multiple += max) {
    const divisible = range.every((value) => multiple % value === 0);
    if (divisible) {
      return multiple;
    }
  }
}

console.log( smallestNum([2, 7]) );
// => 420

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
