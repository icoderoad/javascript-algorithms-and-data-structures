---
id: 60826a79a46e25724b800c62
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 在数组原型上实现 filter 方法
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

在数组原型上实现 filter 方法

为了加深对 filter 方法的理解，现在我们来自己实现一下 Array.prototype.filter() 的方法。使用 for 方法实现 filter 相应的功能 。

注意：纯函数可以改变其作用域内定义的局部变量，但我们最好不要这样做。

今天我们练习编写一个和 Array.prototype.filter() 功能一样的 Array.prototype.iFilter()方法 。具体代码如下所示：

const sites = [
	{ name: '腾讯', domain: "www.qq.com", userNum: 5200 },
	{ name: '京东', domain: 'www.jd.com', userNum: 3210},
	{ name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

Array.prototype.iFilter = function(callback) {
  
  var newArray = [];

  for (let i = 0; i < this.length; i++) {
    if (callback(this[i]) === true) {
      newArray.push(this[i]);
    }
  }

  return newArray;
};

var nSites = sites.iFilter(function(site) {
  return site.userNum <3230;
});

console.log( nSites );
// => 0: {name: "京东", domain: "www.jd.com", userNum: 3210}
// => 1: {name: "路条编程", domain: "www.icoderoad.com", userNum: 150}


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
