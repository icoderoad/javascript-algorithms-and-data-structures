---
id: 5ff54f60a0499822baa6a09d
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用解构赋值从对象、嵌套对象和数组中分配变量
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用解构赋值从对象、嵌套对象和数组中分配变量。

前面文章我们已经介绍过从对象解构赋值，解构赋值的变量与对象属性名称一致。我们也可以在解构的属性后添加冒号和新的变量名来给解构的值赋予一个新的变量名。

还拿昨天例子的对象来举例,下面是指定新的变量名的例子：

const site = { name: '路条编程', domain:'www.icoderoad.com' };
const { name: siteName, domain: siteDomain} = site;
console.log( siteName, 'siteName'); // => 路条编程 siteName
console.log( siteDomain, 'siteDomain'); // => www.icoderoad.com siteDomain

获取到了 site.name 的值并赋值给名为 siteName 的变量。

同样，我们可以将嵌套的对象解构到变量中。

请看以下代码：

const site = {
  manager: { 
  	name:'admin',
    age: 32,
    email: 'admin@icoderoad.com'
  }
};

这是解构对象的属性并赋值给相同名字的变量：

const { manager: { name, age, email }} = site;
console.log(name, age, email ); // => admin 32 admin@icoderoad.com
这是将对象的属性值指定给一个不同的名字：

const { manager: {name: managerName, age: managerAge, email: managerEmail }} = site;
console.log(managerName, managerAge, managerEmail); // => admin 32 admin@icoderoad.com

以上代码解构赋值对象的嵌套属性给变量及新命名的变量，经过比较控制台输出，可以看出，控制输出结果一致。

在 ES6 里面，也可以对数组进行解构赋值操作。解构数组可以如同解构对象一样简单。

与数组解构不同，数组的扩展运算会将数组里的所有内容分解成一个由逗号分隔的列表。所以，你不能选择哪个元素来给变量赋值。

而对数组进行解构却可以让我们做到这一点：

const [numA, numB] = [9, 6, 3, 4, 5, 1];
console.log(numA, numB); // => 9 6

变量 numA 以及  numB分别被数组的第一、第二个元素赋值。 我们甚至能在数组解构中使用逗号分隔符，来获取任意一个想要的值：

const [numA, numB,,, numC] = [9, 6, 3, 4, 5, 1];
console.log(numA, numB, numC); // => 9 6 5

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
