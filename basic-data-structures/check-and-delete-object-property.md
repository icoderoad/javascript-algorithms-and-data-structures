---
id: 603dce0f97d1516b299733ca
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 检查及删除对象属性
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

检查及删除对象属性

前面文章中我们已经学习了新增、修改对象中的属性。如果我们想知道一个对象中是否含有某个属性，应该如何操作呢？JavaScript 语言为我们提供了两种不同的方式来实现这个功能，一个是 hasOwnProperty() 方法，另一个是 in 关键字。如果我们有一个 Sites 对象，它有一个 name  属性，我们可以用以下两种方式之一来检查该属性在对象中是否存在：

Sites.hasOwnProperty('name');

'name' in Sites;

我们已经创建了一个含有一些网站 Sites 对象和一个 getSiteName 方法，该方法接收 key 对象作为参数。检测 Sites 对象中是否存在指定的网站 key, 如果存在，返回网站对象的中文名称，不存在，返回字符串 "非法网站关键字"


let Sites = {
  icoderoad: {
    name: '路条编程',
    domain: 'www.icoderoad.ccom'
  },
  alipay: {
    name: '支付宝',
    domain: '支付宝www.alipay.com'
  },
  qq: {
    name: '腾讯',
    domain: 'www.qq.com'
  },
  cctv: {
    name: '央视网',
    domain: 'www.cctv.com'
  }
};

function getSiteName(key) {
	var name = '';
  if( Sites.hasOwnProperty(key) ){
  		var site = Sites[key];
  		name = site.name;
  }else{
  		name = '非法网站关键字';
  }
  return name;
}

console.log(getSiteName('icoderoad'));
// => 路条编程

console.log(getSiteName('alipay'));
// => 支付宝

console.log(getSiteName('cctv'));
// => 央视网

console.log(getSiteName('toutiao'));
// => 非法网站关键字

到目前为止，我们已经知道什么是对象以及对象的基本特性和用途。总之，对象是以键值对的形式，灵活、直观地存储结构化数据的一种方式，并且查找对象属性的速度很快。

在之前的文章中，我们已经介绍过新增和修改对象中的键值对。现在我们来看如何从一个对象中移除一个键值对。

我们继续为 Sites 对象为例，如果我们想删除 Site 对象的 domain 属性，并返回删除属性后的对象。我们可以使用 delete 关键字：

delete site.domain;

我们定义一个 delSiteDomainByKey 方法，如果不存在指定的 key, 返回 null。完整代码如下所示：

function delSiteDomainByKey(key) {
  if( Sites.hasOwnProperty(key) ){
  		var site = Sites[key];
  		delete site.domain;
  		return site;
  }
  return null;
}

console.log( delSiteDomainByKey('qq') );
// => {name: "腾讯"}

console.log( delSiteDomainByKey('jd') );
// => null

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
