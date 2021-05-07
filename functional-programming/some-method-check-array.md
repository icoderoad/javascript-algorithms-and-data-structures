---
id: 6094d1331b00ae09f4a5a426
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用数组 some 方法检查数组中是否有元素符合指定条件
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

使用数组 some 方法检查数组中是否有元素符合指定条件

在介绍具体示例之前，先介绍下 some() 方法的具体用法。

some() 方法测试数组中是不是至少有1个元素通过了被提供的函数测试。它返回的是一个Boolean类型的值。

注意：如果用一个空数组进行测试，在任何情况下它返回的都是false。

语法:
	arr.some(callback(element[, index[, array]])[, thisArg])

参数:
	callback
		用来测试每个元素的函数，接受三个参数：
		element
			数组中正在处理的元素。
		index 可选
			数组中正在处理的元素的索引值。
		array可选
			some()被调用的数组。

	thisArg可选
		执行 callback 时使用的 this 

返回值:
	数组中有至少一个元素通过回调函数的测试就会返回 true；所有元素都没有通过回调函数的测试返回值才会为 false。

描述:
	some() 为数组中的每一个元素执行一次 callback 函数，直到找到一个使得 callback 返回一个“真值”（即可转换为布尔值 true 的值）。如果找到了这样一个值，some() 将会立即返回 true。否则，some() 返回 false。callback 只会在那些”有值“的索引上被调用，不会在那些被删除或从来未被赋值的索引上调用。

	callback 被调用时传入三个参数：元素的值，元素的索引，被遍历的数组。

	如果一个 thisArg 参数提供给 some()，它将被用作调用的 callback的 this 值。否则， 它的 this value将是 undefined。this 的值最终通过 callback 来观察，根据 the usual rules for determining the this seen by a function的 this 判定规则来确定。

	some() 被调用时不会改变数组。

	some() 遍历的元素的范围在第一次调用 callback. 前就已经确定了。在调用 some() 后被添加到数组中的值不会被 callback 访问到。如果数组中存在且还未被访问到的元素被 callback 改变了，则其传递给 callback 的值是 some() 访问到它那一刻的值。已经被删除的元素不会被访问到。

我们来练习一个完整的示例，下面的代码检测网站数组  sites 的员工数是否都小于 3000。我们定义一个方法 checkSiteUserNum(), 参数为 sites,返回值为布尔值，是否员工数有小于 3000 的。
 
const sites = [
  { name: '腾讯', domain: 'www.qq.com', userNum: 5200 },
  { name: '京东', domain: 'www.jd.com', userNum: 3210},
  { name: '天猫', domain: 'www.tmall.com', userNum: 4231},
  { name: '路条编程', domain: 'www.icoderoad.com', userNum:150 }
];

function checkSiteUserNum(arr) {

  return arr.some(function(site) {
  	return site.userNum <3000;
  });

}

console.log( checkSiteUserNum( sites ) );
// => true

以上代码执行后，在控制台输出 true ,说明网站数组中的网站员工数有小于 3000 人的。

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
