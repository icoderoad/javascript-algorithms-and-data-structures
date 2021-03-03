---
id: 603f1e8a8c26b742e03fb093
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 for...in 语句迭代对象
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 for...in 语句迭代对象

有时候在开发过程中需要遍历一个对象中的所有键。这需要 JavaScript 中的一个特殊语法：for...in 语句。以遍历 Sites 对象的键为例：

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

for (let site in Sites) {
  console.log( site );
}

// =>
163
icoderoad
alipay
sohu
qq
cctv
weibo

在这个语句中，我们定义了一个 site 变量，您可以看到，这个变量在 for...in 语句中对对象的每一个键的遍历都会被重置。

注意：跟数组不同，对象中的键是无序的，因此一个对象中某个键的位置，或者说它出现的相对顺序，在引用或访问该键时是不确定的。

下面我们做个练习，定义了一个 getTotalNumByDomain 方法，使用 for...in 语句来遍历 Sites 对象中的网站信息，并返回包含域名 domain 属的网站数量。

function getTotalNumByDomain( sites ){
  let total = 0;
  for (let siteKey in sites) {
      var siteObj = sites[siteKey];
      if( siteObj.hasOwnProperty( 'domain' ) ){
          total++;
      }
  }
  return total;
}

console.log('共有包含域名的网站数：' + getTotalNumByDomain( Sites ));
// => 共有包含域名的网站数：4

以上代码我们定义了方法 getTotalNumByDomain， 其中参数 sites 为站点对象。方法中定义了变量 total, 初始值为 0 ，通过 for...in 语句循环 sites 对象里的网站对象，通过对象的 hasOwnProperty 方法判断对象中是否包含指定属性  domain, 如果包含 total 变量值 + 1，最终将 total 变量返回。在控制台将 getTotalNumByDomain 方法返回值输出，最终控制台输出为 “共有包含域名的网站数：4”。

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
