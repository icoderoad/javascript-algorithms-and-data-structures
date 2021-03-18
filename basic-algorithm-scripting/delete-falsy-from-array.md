---
id: 605317758e2252571023286f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 删除数组中的所有虚值
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

删除数组中的所有虚值

今天我们介绍如何删除数组中的所有虚值的方法。。在介绍具体方法之前，我们先介绍下 falsy 值 (虚值)

falsy 值 (虚值) 是在 Boolean 上下文中认定为 false 的值。

JavaScript 在需要用到布尔类型值的上下文中使用强制类型转换(Type Conversion )将值转换为布尔值，例如条件语句和循环语句。

在 JavaScript 中只有 8 个 falsy 值。

这意味着当 JavaScript 期望一个布尔值，并被给与下面值中的一个时，它总是会被当做 false。

false			false 关键字
0				数值 zero	
-0				数值 负 zero	
0n				当 BigInt 作为布尔值使用时, 遵从其作为数值的规则. 0n 是 falsy 值.
				"", '', ``	
				这是一个空字符串 (字符串的长度为零). JavaScript 中的字符串可用双引号 "", 单引号 '', 或 模板字面量 `` 定义。

null			null - 缺少值
undefined		undefined - 原始值
NaN	NaN 		- 非数值


实现步骤如下所示：

1、创建一个新数组，保存原数组里的真值数据

2、通过 for 循环确定 arr 中的哪些值是虚值。

3、遍历数组元素，如果元素不为虚值，添加至数组里

4、返回仅包含真值（truthy）的新数组。

具体代码如下所示：

function falsyArr(arr) {
  let newArray = [];
  for (let i = 0; i < arr.length; i++) {
    if (arr[i]) newArray.push(arr[i]);
  }
  return newArray;
}

console.log( falsyArr([111, "icoderoad", "路条编程", false, 0])  );
// => (3) [111, "icoderoad", "路条编程"]

console.log( falsyArr([-0, "On", "路条公众号", null, undefined, NaN])  );
// => ["On", "路条公众号"]



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
