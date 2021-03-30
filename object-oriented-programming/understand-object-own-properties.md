---
id: 605ec475401d938a63e35759
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 了解对象自身属性
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

了解对象自身属性

请看下面的实例，Site 构造函数定义了两个属性：name 和 address

function Site(name) {
  this.name  = name;
  this.address = "北京市海淀区";
}

let icodeRoadSite = new Site("路条编程");

let qqSite = new Site("腾讯");

name 和 address 被叫做自身属性，因为他们是直接在实例对象上定义的。这就意味着 icodeRoadSite  和 qqSite 这两个对象分别拥有这些属性的独立副本。 Site  以下的代码将 icodeRoadSite 里面所有的自身属性都存到一个叫ownProps的数组里面：

let ownProps = [];
for (let property in icodeRoadSite) {
  if( icodeRoadSite.hasOwnProperty(property)) {
    ownProps.push(property);
  }
}

console.log(ownProps); 
// => (2) ["name", "address"]


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
