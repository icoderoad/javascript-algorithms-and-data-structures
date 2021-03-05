---
id: 60406e6f80922c61032a6474
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 Object.Keys() 生成对象所有键组成的数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 Object.Keys() 生成对象所有键组成的数组

我们还可以输入一个对象作为参数来调用 Object.keys()方法，使其生成一个包含对象中所有键的数组。这会返回一个由对象中所有键的名称（字符串）组成的数组。再次说明，这个数组中的项的顺序是不确定的。

Object.keys 方法返回一个所有元素为字符串的数组，其元素来自于从给定的 object 上面可直接枚举的属性。这些属性的顺序与手动遍历该对象属性时的一致。


语法：Object.keys(obj)

参数：obj 要返回其枚举自身属性的对象。

返回值：一个表示给定对象的所有可枚举属性的字符串数组。

下面我们做个练习，定义一个 getArrayFromSitesKey 方法，使其返回一个包含输入的对象的所有属性的数组。


let Sites = {
  icoderoad: {
    name: '路条编程',
    domain: 'www.icoderoad.ccom'
  },
  alipay: {
    name: '支付宝',
    domain: '支付宝www.alipay.com'
  },
  sohu: {
    name: '搜狐',
    address:'北京市'
  },
  qq: {
    name: '腾讯',
    domain: 'www.qq.com'
  },
  163:{
    name: '网易',
    address:'北京市'
  },
  cctv: {
    name: '央视网',
    domain: 'www.cctv.com'
  },
  weibo: {
    name: '微博',
    address:'北京市'
  }
};

function getArrayFromSitesKey( obj ) {
  return Object.keys(obj);
}

console.log(getArrayFromSitesKey( Sites ));
// => (7) ["163", "icoderoad", "alipay", "sohu", "qq", "cctv", "weibo"]

以上代码定义了方法 getArrayFromSitesKey， 参数为 obj, getArrayFromSitesKey，方法中调用 Object.keys 方法，返回 obj 对象所有属性组成的新数组。将返回值打印在控制台，控制台最终输出结果为 ‘(7) ["163", "icoderoad", "alipay", "sohu", "qq", "cctv", "weibo"]’。
经过输出结果比较，我们可以发现返回数组中的值为 Sites 对象的所有属性值。


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
