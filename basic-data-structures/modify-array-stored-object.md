---
id: 6041c1929fc8764ca0a36424
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 修改存储在对象中的数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

修改存储在对象中的数组

到目前为止，我们已经介绍了 JavaScript 语言对象的所有运算。可以增加、修改和移除键值对，检查某个键是否存在，也可以遍历一个对象中的所有键。在继续学习 JavaScript 语言的过程中，大家会看到对象的更多用法。另外，后续的《高级数据结构》专题还会介绍 ES6 的 Map 和 Set 对象。这两种对象都跟一般的对象相似，但它们提供了一些额外的特性。现在大家已经学到了数组和对象的基础知识，我们已经可以继续用 JavaScript 语言来解决更加复杂的问题了！

请大家看一下下面代码部分我们提供的对象。user 对象包含 3 个键。data 对象包含 6 个键，其中包含一个 followers 数组。从这个例子可以看到对象作为数据结构是多么的灵活。我们通过 addFollower 方法为 user 对象添加关注者，将 follower 参数中的名字添加到 user.data.followers 数组中并返回该数组。

let user = {
  name: '路条小白',
  age: 21,
  data: {
    userName: 'icoderoad',
    createDate: '2021-03-04 10:28:05',
    email: 'admin@icoderoad.cocm',
    company: '路条科技',
    followers:[
      '李华',
      '王宁',
      '孟飞'
    ],
    location: {
      city: '北京',
      country: '中国'
    }
  }
};

function addFollower(mUser, follower) {
  mUser.data.followers.push(follower);
  return mUser.data.followers;
}

let followers = addFollower(user, '赵云');
console.log(followers);
// => (4) ["李华", "王宁", "孟飞", "赵云"]

以上代码我们定义了一个 user 对象 和一个添加关注者的方法，addFollower 方法包含两个参数，用户对象 user 和关注者 follower，此方法将关注者添加至 user 对象的关注者数组 followers， 并将添加关注者后的数组返回。我们给用户新增了一个新的关注者 ‘赵云’，然后将添加后的关注者数组赋值给变量 followers，最终将 followers 在控制台打印输出，输出结果为 ‘(4) ["李华", "王宁", "孟飞", "赵云"]’。根据控制台输出结果可知，新的关注者已经添加至用户 user 的关注者数组。

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
