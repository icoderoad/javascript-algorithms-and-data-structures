---
id: 60a744a94824455d05056330
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 计算所有小于或等于指定数字的质数之和

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

计算所有小于或等于指定数字的质数之和

本次练习我们需要写一个函数 sumPrimes ，参数为一个正整数 num。该函数返回所有小于或等于该数字的质数之和。

质数是大于 1 且仅可以被 1 和自己整除的数。 比如，2 就是一个质数，因为它只可以被 1 和 2（它本身）整除。 相反，4 不是质数，因为它可以被 1, 2 和 4 整除。

在介绍完整代码之前，我们先介绍下数组 every 方法的具体用法： 

every() 方法测试一个数组内的所有元素是否都能通过某个指定函数的测试。它返回一个布尔值。

注意：若收到一个空数组，此方法在一切情况下都会返回 true。

语法:
arr.every(callback(element[, index[, array]])[, thisArg])

参数:
  callback
    用来测试每个元素的函数，它可以接收三个参数：
    element
      用于测试的当前值。
    index可选
      用于测试的当前值的索引。
    array可选
      调用 every 的当前数组。
    thisArg
    执行 callback 时使用的 this 值。

返回值:
如果回调函数的每一次返回都为 truthy 值，返回 true ，否则返回 false。

every 方法为数组中的每个元素执行一次 callback 函数，直到它找到一个会使 callback 返回 falsy 的元素。如果发现了一个这样的元素，every 方法将会立即返回 false。否则，callback 为每一个元素返回 true，every 就会返回 true。callback 只会为那些已经被赋值的索引调用。不会为那些被删除或从未被赋值的索引调用。

callback 在被调用时可传入三个参数：元素值，元素的索引，原数组。

如果为 every 提供一个 thisArg 参数，则该参数为调用 callback 时的 this 值。如果省略该参数，则 callback 被调用时的 this 值，在非严格模式下为全局对象，在严格模式下传入 undefined。详见 this 条目。

every 不会改变原数组。

every 遍历的元素范围在第一次调用 callback 之前就已确定了。在调用 every 之后添加到数组中的元素不会被 callback 访问到。如果数组中存在的元素被更改，则他们传入 callback 的值是 every 访问到他们那一刻的值。那些被删除的元素或从来未被赋值的元素将不会被访问到。

练习完整代码如下所示：

function sumPrimes(num) {
  let primes = [];
  for (let i = 2; i <= num; i++) {
    if (primes.every((prime) => i % prime !== 0))
      primes.push(i);
  }
  return primes.reduce((sum, prime) => sum + prime, 0);
}

console.log( sumPrimes(32) );
// => 160

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
