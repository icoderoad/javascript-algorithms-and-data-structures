---
id: 6000efffb5c44449b8acce0b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过 Promise 进行异步编程及成功方法 resolve 和失败方法 reject 介绍
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
通过 Promise 进行异步编程及成功方法 resolve 和失败方法 reject 介绍。

Promise 是异步编程的一种解决方案 - 它在未来的某时会生成一个值。任务完成，分执行成功和执行失败两种情况。一个 Promise 对象代表一个在这个 promise 被创建出来时不一定已知的值。它让您能够把异步操作最终的成功返回值或者失败原因和相应的处理程序关联起来。 这样使得异步方法可以像同步方法那样返回值：异步方法并不会立即返回最终的值，而是会返回一个 promise，以便在未来某个时候把值交给使用者。

一个 Promise 必然处于以下几种状态之一：

待定（pending）: 初始状态，既没有被兑现，也没有被拒绝。
已兑现（fulfilled）: 意味着操作成功完成。
已拒绝（rejected）: 意味着操作失败


注意： 如果一个 promise 已经被兑现（fulfilled）或被拒绝（rejected），那么我们也可以说它处于已敲定（settled）状态。您还会听到一个经常跟 promise 一起使用的术语：已决议（resolved），它表示 promise 已经处于已敲定(settled)状态，或者为了匹配另一个 promise 的状态被"锁定"了。

Promise 是构造器函数，需要通过 new 关键字来创建。构造器参数是一个函数，该函数有两个参数 - resolve 和 reject。通过它们来判断 promise 的执行结果。用法如下所示：

const promise = new Promise((resolve, reject) => {

});

上面我们介绍了 promise 有三个状态，分别为 pending、fulfilled 和 rejected。promise 提供的 resolve 和 reject 参数就是用来结束 promise 的。promise 成功时调用 resolve，promise 执行失败时调用 reject，这两个方法接收一个参数，如下所示。

const promise = new Promise((resolve, reject) => {
  if(条件判断) {
    resolve("Promise 已兑现 ");
  } else {
    reject("Promise 被拒绝");
  }
});

上面的例子使用字符串做为函数的参数，也可以是任意类型，通常是使用对象，里面可能是将要放到页面或其它地方的数据。

下面我们练习一个完整的例子，创建一个变更为 userRequest 的 Promise 对象。代码如下所示：

const userRequest = new Promise((resolve, reject) => {
  let succ;
    
  if( succ ) {
    resolve("用户数据获取成功")
  } else {  
   reject("用户数据获取失败")
  }
});

使 promise 可以处理成功和失败情况。如果 succ 是 true，调用 resolve 方法使 promise 成功。给 resolve 传递值为 用户数据获取成功 的字符串。如果 succ 是 false， 使用 reject 方法并传入值为 用户数据获取失败 的字符串。

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
