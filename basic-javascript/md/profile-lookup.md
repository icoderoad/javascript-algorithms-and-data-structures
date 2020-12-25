---
id: 5fe4282a8f0d3a1caedf4691
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通讯录查找联系人功能简单实现
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
通讯录查找联系人功能简单实现。

经过这段时间的学习，我们对 JavaScript 语言基础知识有了比较全面的了解，根据我们所学的知识，我们实现一个用户资料查找的简单功能。我们有一个对象数组，里面存储着用户通讯录信息。通过函数 lookUpProfile 实现用户通讯录信息查找。

函数 lookUpProfile 有两个预定义参数：name 值和 prop 属性。函数将会检查通讯录中是否存在一个与传入的 name 参数值相同的联系人。如果存在，还需要检查对应的联系人中是否存在 prop 属性。如果它们都存在，函数返回 prop 属性对应的值。如果 name 值不存在，返回 "通讯录中没有对应联系人"。如果 prop 属性不存在，返回 "没有查找属性"。

如果判断一个对象中是否含有相应属性呢？我们可以用对象的 hasOwnProperty(propName) 方法来检查对象是否有该属性。如果有返回 true，反之返回 false 。


var user = {
  name: "hat",
  phone: "pants",
  hobby: ["读书","上网", "听音乐"]
};
console.log(user.hasOwnProperty("name")) ; // => true
console.log(user.hasOwnProperty("address")); // => false

以上代码定义了一个用户对象 user ,包含 name、phone、hobby 三个属性，分别表示用户的姓名、电话及爱好。通过 user 对象的 hasOwnProperty 属性判断 name 和 address 属性是否存在，控制台分别输出 true 和 false。

以下代码为一个通讯录查找联系人功能：

var contacts = [
    {
        "name": "黄宇",
        "phone": "157652xxxx1",
        "hobby": ["足球", "音乐", "旅游"]
    },
    {
        "name": "金飞",
        "phone": "189043xxxx2",
        "hobby": ["体育", "看电影", "红酒"]
    },
    {
        "name": "王东",
        "phone": "178034xxxx3",
        "hobby": ["打游戏", "理财"]
    },
    {
        "name": "周贺",
        "phone": "190765xxxx4",
        "hobby": ["编码", "打游戏", "抽烟"]
    }
];


function lookUpProfile(name, prop){
  var found = false;
  var result = "";
  var userObj = {};
  for( var i=0;i<contacts.length; i++ ){
    var user = contacts[i];
    if( user.name === name ){
        found = true;
        userObj= user;
        break;
    }
  } 
  if( found ){
    if( userObj.hasOwnProperty( prop ) ){
      result = userObj[prop];
    }else{
      result = "没有查找属性";
    }
  }else{
    result = "通讯录中没有对应联系人";
  }
  return result;
}

console.log( lookUpProfile("周贺", "hobby") ); // => ["编码", "打游戏", "抽烟"]
console.log( lookUpProfile("黄宇", "address") ); // => 没有查找属性
console.log( lookUpProfile("赵健", "hobby") ); // => 通讯录中没有对应联系人

以上代码定义了一个联系人数组 contacts， 数组包含 4 个联系人对象，每个联系人包含 name、phone、hobby 三个属性。定义一个函数 lookUpProfile，函数包含 name、prop 两个参数 ，通过 for 循环对联系人数组进行遍历，根据给定的 name 和每个联系人的 name 属性进行比较，如果相等, 将 found 变量设置为 true, 将 user 对象赋值给变量 userObj ，退出循环。 for 循环结束后，根据 found 进行相应逻辑判断。如果 found 为 true,  userObj 包含查找属性 ，设置对象属性值，不包含属性值，设置 "没有查找属性" 至变量 result。 最终返回 result 变量。如果 found 为 false, 设置"通讯录中没有对应联系人"给变量 result。

三次调用函数 lookUpProfile ，将结果在控制台输出。最终传入参数及控制台输出结果，参见上面代码及注释部分。

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
