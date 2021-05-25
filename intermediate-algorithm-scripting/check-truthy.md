---
id: 60a83a8be9d4771ecacc0778
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 检查集合所有元素是否都是真值

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

检查集合所有元素是否都是真值

本次练习我们需要写一个函数 checktruthy ，它接收两个参数 arr, prop，如果参数1 数组中的所有元素都为真，方法返回真 ，否则返回假。
 
参数arr 为集合元素，参数 prop 是一个对象的属性，如果它的值是 truthy（真实的） ，则返回 true，否则，返回 false 。

JavaScript 中，如果一个值在 Boolean 的上下文中（比如if语句）可以被执行为 true，那么这个值就被认为是 truthy 的。

注意，可以选择使用.或[]来访问对象属性对应的值。

在介绍完整代码之前，我们先介绍下数组 hasOwnProperty 方法的具体用法： 

hasOwnProperty() 方法会返回一个布尔值，指示对象自身属性中是否具有指定的属性（也就是，是否有指定的键）。

语法：
obj.hasOwnProperty(prop)

参数：
prop
要检测的属性的 String 字符串形式表示的名称，或者 Symbol。

返回值：
用来判断某个对象是否含有指定的属性的布尔值 Boolean。

练习完整代码如下所示：

function checktruthy(arr, prop) {
   var counter = 0;
  for (var c in arr) {
  
    if (arr[c].hasOwnProperty(prop) && Boolean(arr[c][prop])) {
      counter++;
    }
  }
  
  return counter == arr.length
}

console.log( checktruthy( [{"user": "王飞", "sex": "男"}, {"user": "李健"}, {"user": "韩红", "sex": "女"}, {"user": "牛一", "sex": "男"}], "sex" ));
// => false

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
