---
id: 5feef95e09ee7101ea551156
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过 Object.freeze() 方法防止对象改变
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
通过 Object.freeze() 方法防止对象改变。

前面的文章中我们介绍过，const 关键字声明的变量并不会真的保护数据不被改变。为了确保数据不被改变，JavaScript 语言提供了一个 Object.freeze() 方法来防止数据改变。

Object.freeze() 方法可以冻结一个对象。一个被冻结的对象再也不能被修改；冻结了一个对象则不能向这个对象添加新的属性，不能删除已有属性，不能修改该对象已有属性的可枚举性、可配置性、可写性，以及不能修改已有属性的值。此外，冻结一个对象后该对象的原型也不能被修改。freeze() 返回和传入的参数相同的对象。

语法：
Object.freeze( obj )

参数：
obj：要被冻结的对象。

返回值:
被冻结的对象。

当一个对象被冻结的时候，不能再对它的属性再进行增、删、改的操作。任何试图改变对象的操作都会被阻止，却不会报错。

let objFreeze = {
  name:"路条编辑",
  address:"北京市朝阳区"
};

Object.freeze(objFreeze);

objFreeze.address = "湖北省武汉市"; // 此操作将被忽略，也不报错
objFreeze.tel = "010-86750100"; // 此操作将被忽略，也不报错
console.log(objFreeze); // => {name: "路条编辑", address: "北京市朝阳区"}

上面代码声明了一个对象 objFreeze， 包含 name、address 两个属性，初始化时设置名称 name 属性为 "路条编辑"， 地址 address 属性为 "北京市朝阳区"。然后执行冻结操作，修改地址 address 属性为 "湖北省武汉市"， 增加电话 tel 属性，然后在控制台输出对象，控制台输出结果为 {name: "路条编辑", address: "北京市朝阳区"}。由此可见，对象执行 freeze 方法后，不能再操作此对象。

下面我们练习一个复杂的示例，我们将使用 Object.freeze 方法来防止数学常量被改变。需要冻结 MATH_CONSTANTS 对象，使得任何人不可以改变 PI 的值，不能增加或删除  ATH_CONSTANTS 对象的属性。示例代码如下所示：

function freezeObj() {
  'use strict';
  const MATH_CONSTANTS = {
    PI: 3.14
  };
  // comment placeholder (needs translation)

  Object.freeze( MATH_CONSTANTS );
  // comment placeholder (needs translation)
  try {
    MATH_CONSTANTS.PI = 66;
  } catch(ex) {
    console.log(ex);
  }
  return MATH_CONSTANTS.PI;
}
const PI = freezeObj();

console.log( PI );// => typeError: Cannot assign to read only property 'PI' of object '#<Object>'
// => 3.14

以上代码定义了一个冻结对象方法 freezeObj， 先声明对象 MATH_CONSTANTS ，设置属性 PI 值为 3.14 ，冻结 MATH_CONSTANTS ，然后修改 MATH_CONSTANTS 对象的属性 PI 值为 66， 返回对象 PI 属性。调用函数 freezeObj 赋值给变量 PI ，在控制台输出 PI 变量。控制台会输出两行信息，第一行显示类型错误，第二行显示值为 3.14。 

示例说明通过 Object.freeze() 方法冻结的对象，不能再对其做任何修改，可以实现防止对象改变的目的。

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
