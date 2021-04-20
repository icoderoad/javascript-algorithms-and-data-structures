---
id: 607e68840020c4ed3ece9e52
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 在函数中重构全局变量

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

在函数中重构全局变量

目前为止，我们已经看到了函数式编程的两个原则：

1) 不要更改变量或对象——创建新变量和对象，并在需要时从函数返回它们。

2) 声明函数参数——函数内的任何计算仅取决于参数，而不取决于任何全局对象或变量。

给数字增加 1 不够刺激，我们可以在处理数组或更复杂的对象时应用这些原则。

重构代码，使全局数组 userList 在函数内部不会被改变。add 函数可以将指定的 userName 增加到数组末尾。remove 函数可以从数组中移除指定 userName。两个函数都返回数组，并且任何参数都应该添加到 userName 前面。

var userList = ["王飞", "李婷", "于牛", "丁晓"];

function add(arr, userName) {
  let newArr = [...arr]; 
  newArr.push(userName); 
  return newArr; 
}

function remove(arr, userName) {
  let newArr = [...arr]; 
  if (newArr.indexOf(userName) >= 0) {
    newArr.splice(newArr.indexOf(userName), 1); 
    return newArr; 
  }
}

var userList1 = add(userList, "韩非");
var userList2 = remove(userList, "纪明");
var userList3 = remove(add(userList, "蔡猛"),"张在");

console.log(userList);
// => (4) ["王飞", "李婷", "于牛", "丁晓"]


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
