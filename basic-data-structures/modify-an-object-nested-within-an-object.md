---
id: 603ad83d8fc8972a00f128d1
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 修改嵌套在对象中的对象
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

修改嵌套在对象中的对象

今天我们来看一个稍微复杂一点的对象。对象中也可以嵌套任意层的对象。对象的属性值可以是 JavaScript 语言支持的任意类型，包括数组和其他对象。示例代码如下所示：

let mSiteObj = {
  id: 111,
  name: '路条编程',
  data: {
    userNum: 999,
    activeUsers: 888,
    project: {
      nums: 120,
      completes: 99
    }
  }
};

mSiteObj 3 个唯一的键：值为一个数字的 id、值为一个字符串的 name  和值为一个嵌套了其他对象的对象的 data。虽然对象中的数据可能很复杂，我们仍能使用上篇文章中讲的符号来访问我们需要的信息。

下面我们使用之前介绍的方式来修改被嵌套的对象的属性。将项目对象的总数 nums 修改为 360， 完成数 completes 修改为 320，然后打印相应的对象到控制台。

mSiteObj.data.project.nums=360;
mSiteObj.data.project.completes=320

console.log(mSiteObj);
// => 
{
	data:
		activeUsers: 888
		project:
			completes: 320
			nums: 360
			userNum: 999
	id: 111
	name: "路条编程"
}

根据控制台的输出结果可知，project 对象下面的 completes 和 nums 属性已经被修改为 360 和 320。

也可以通过下面的方式来修改对象的值

mSiteObj['data']['activeUsers'] = 890;

console.log( mSiteObj );
// => {
	data:
		activeUsers: 890
		project: {nums: 360, completes: 320}
		userNum: 999

	id: 111
	name: "路条编程"
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
