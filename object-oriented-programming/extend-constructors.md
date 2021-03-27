---
id: 605ec475401d938a63e35759
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用带有参数的对象构造函数创建对象
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用带有参数的对象构造函数创建对象

上篇文章中我们介绍了 Site 对象构造函数及创建对象相关的知识，对象可以正常创建并运行。不知大家在执行程序的过程中注意到此程序的限制了吗？就是所有通过 Site  构造函数创建出来的实例  codeRoadSite 都自动的取名为 路条编程，域名都是 www.icoderoad.com ，地址都是 北京市海淀区。如果想要新创建出来的站点拥有不同的名字和域名我们要怎么办呢？当然，创建实例后手动去修改每一个站点实例名称和域名属性也是可以实现的，只是会增加很多无谓的工作量,类似下面的代码实现：

function Site() {
  this.name = "路条编程";
  this.domain = "www.icoderoad.com";
  this.address = "北京市海淀区";
   // 构造器内的 "this" 一直指向创建的对象
}

let codeRoadSite = new Site();
codeRoadSite.name = "腾讯";
codeRoadSite.domain = "www.qq.com";

console.log(codeRoadSite.name); 
// => 腾讯

console.log(codeRoadSite.domain); 
// => www.qq.com


假如写了一个程序来查询一个北京市海淀区站点集合里面的几百个甚至几千个不同的站点，将会花费很多时间去创建所有的站点实例并给它们的属性一一修改为不同的值。 为了减轻创建不同 Site 对象的工作量，咱们可以给 Site 对象增加带参数的构造函数，代码实现如下所示：

function Site(name, domain) {
  this.name = name;
  this.domain = domain;
  this.address = "北京市海淀区";
}

然后将值通过参数的方式传递给 Site 构造函数来定义每一个唯一的站点实例： 

let site = new Site("央视网", "www.cctv.com"); 

这给 Site 的名字和域名属性分别赋值为 央视网 和 www.cctv.com 提供了另外一种方法。地址属性被默认赋值为 北京市海淀区。 site 有以下这些属性：

console.log(site.name );
// => 央视网

console.log(site.domain );
// => www.cctv.com

console.log(site.address );
// => 北京市海淀区

这样一来构造函数就变得很灵活了。现在可以直接定义每个 Site 实例在创建时的属性，这是 JavaScript 构造函数非常实用的用法之一。它们根据共同或相似的属性和行为将对象归纳为一组，并能够自动的创建各自实例。


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
