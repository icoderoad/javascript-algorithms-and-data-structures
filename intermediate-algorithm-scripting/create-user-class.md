---
id: 60ac8e7858bf91ecfc484e21
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 创建一个用户类

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

创建一个用户类

本次练习我们需要写构造器（constructor）函数，它只接收两个参数 name、sex ，分别代表用户名和性别。这个构造函数创建出的实例需要具有以下方法：

getNameString()
getName()
getSex()
setName(name)
setSex(sex)

然后就可以在浏览器控制台中看到每个测试用例执行的情况。 方法接收一个字符串格式的参数。 这些方法必须是与对象进行交互的唯一可用方法。

在介绍完整代码之前，我们先介绍下 构造函数 方法的具体用法： 

构造函数
  Function 构造函数创建一个新的 Function 对象。直接调用此构造函数可用动态创建函数，但会遇到和 eval 类似的的安全问题和(相对较小的)性能问题。然而，与 eval 不同的是，Function 创建的函数只能在全局作用域中运行。

语法：
  new Function ([arg1[, arg2[, ...argN]],] functionBody)

参数：
  arg1, arg2, ... argN
  被函数使用的参数的名称必须是合法命名的。参数名称是一个有效的JavaScript标识符的字符串，或者一个用逗号分隔的有效字符串的列表;例如“×”，“theValue”，或“a,b”。
  functionBody

一个含有包括函数定义的 JavaScript 语句的字符串。

使用 Function 构造器生成的 Function 对象是在函数创建时解析的。这比你使用函数声明或者函数表达式并在你的代码中调用更为低效，因为使用后者创建的函数是跟其他代码一起解析的。

所有被传递到构造函数中的参数，都将被视为将被创建的函数的参数，并且是相同的标示符名称和传递顺序。

以调用函数的方式调用 Function 的构造函数（而不是使用 new 关键字) 跟以构造函数来调用是一样的。


练习完整代码如下所示：

function User(name, sex) {
  var mName = name;
  var mSex = sex;

  this.getName = function() {
    return mName;
  };

  this.getNameString = function() {
    return "姓名：" + mName + ", 性别:" + mSex;
  };

  this.getSex = function() {
    return mSex;
  };

  this.setSex = function(sex) {
    mSex = sex;
  };

  this.setName = function(name) {
    mName = name;
  };

}

var user = new User("路条小白", "男");
console.log( user.getNameString());
// => 姓名：路条小白, 性别:男

console.log("姓名：" + user.getName());
// => 姓名：路条小白

console.log("性别：" + user.getSex());
// => 性别：男

user.setName("路条小白2");
user.setSex("女");

console.log( user.getNameString());
// => 姓名：路条小白2, 性别:女

console.log("姓名：" + user.getName());
// => 姓名：路条小白2

console.log("性别：" + user.getSex());
// => 性别：女

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
