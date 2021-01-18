---
id: 60040ff36688132f49c52103
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过 then  和 catch 处理 Promise 完成及失败的情况
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
通过 then  和 catch 处理 Promise 完成及失败的情况。

当程序需要花费未知的时间才能完成时 Promise 很有用（比如，一些异步操作），一般是网络请求。网络请求会花费一些时间，当结束时需要根据服务器的响应执行一些操作。这可以用 then 方法来实现，当 promise 完成 resolve 时会触发 then 方法。示例代码如下所示：

promise.then(result => {
  // 结果中执行一些相应操作
  console.log( result );
});
result 即传入 resolve 方法的参数。

给 promise 添加 then 方法。用 result 做为回调函数的参数并将 result 打印在控制台。

当 promise 失败时会调用 catch 方法。当 promise 的 reject 方法执行时会直接调用。用法示例如下所示：

promise.catch(error => {
  // promise 出错时执行一些相应错误处理操作
});
error 是传入 reject 方法的参数。

注意： then 和 catch 方法可以在 promise 后面链式调用。

我们继续完善之前介绍的 promise 操作示例，

const userRequest = new Promise((resolve, reject) => {
  let succ;
    
  if( succ ) {
    resolve("用户数据获取成功")
  } else {  
   reject("用户数据获取失败")
  }
});

userRequest.then(result => {
  console.log( result );
}).catch( error =>{
  console.log( error );
});

上面代码给 promise 添加 then 和 catch 方法。用 result 和 error 做为 then 和 catch 回调函数的参数并把 result 和 error 打印到控制台。

到今天为止，我们 ES6 基础知识部分的内容就讲完了，下面我们继续学习 正则表达式 专题相关的知识。感兴趣的同学请继续关注公众号，每天准时发送。
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
