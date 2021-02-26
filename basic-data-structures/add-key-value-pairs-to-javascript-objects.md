---
id: 6039870da4910628cc946c73
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将键值对添加到对象中
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

将键值对添加到对象中

对象（object）本质上是键值对（key-value pair）的集合，或者说，一系列被映射到唯一标识符或叫做属性（property）或叫键（key））的数据。让我们来看一个很简单的例子：

let ICR_User = {
  userName: 'icoderoad',
  name: '路条编程',
  sex: '男',
  mail: 'admin@icoderoad.com'
};

上面的代码定义了一个叫做 ICR_User 的对象，它有 4 个属性，每个属性映射一个特定的值。如果我们想知道 ICR_User 的邮箱是什么，我们可以这样访问其 mail 属性：

let mail = ICR_User.mail;
console.log( mail );
// => admin@icoderoad.com

这叫做点符号。我们还可以用方括号符号来访问对象中的属性：

let name = ICR_User['name'];
console.log( name );
// => 路条编程

注意，在用方括号符号时，我们在括号里写的是字符串 name（用引号括起）。方括号符号让我们能用一个变量作为属性名来访问对象的属性。若我们在方括号中不写引号而直接写 name ，JavaScript 语言引擎会将其看作一个变量，并抛出一个 ReferenceError: followers is not defined 的错误。

用这样的语法，我们还可以向对象中新增键值对。我们已经创建了一个有 3 个属性的 Site 对象，请为其新增 3 项：值为 12 的  staff 属性、值为 010-88420000 的 telphone 属性和值为 010-88420001 的 fax 属性。

let Site = {
  name: '路条编程',
  domain: 'www.icoderoad.com',
  address: '北京市朝阳区大望路'
};

Site['staff']= 12;
Site['telphone']= '010-88420000';
Site['fax']= '010-88420001';

console.log(Site);

// => {
address: "北京市朝阳区大望路"
domain: "www.icoderoad.com"
fax: "010-88420001"
name: "路条编程"
staff: 12
telphone: "010-88420000"
}


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
