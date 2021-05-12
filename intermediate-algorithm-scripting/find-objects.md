---
id: 609b6d2d7dd5941633b6a37f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 从对象数组中找出与相等或包含的所有对象方法实现
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

从对象数组中找出与相等或包含的所有对象方法实现

本次练习我们需要写一个函数 findObjectInArrays 。该方法接收两个参数：第一个参数是对象数组 objs，第二个参数是一个对象 obj。我们需要从对象数组中找出与第二个参数相等或包含第二个参数的所有对象，并以对象数组的形式返回。

其中，相等的意思是原数组中的对象与第二个参数中对象的所有键值对完全相等；包含的意思是只要第二个参数中对象的所有键存在于原数组对象中，且它们对应的值相同即可。

比如，如果第一个参数是[{ domain: "www.icoderoad.comn", name: "路条编程" }, { domain: "www.tmall.com", name: null }, { domain: "www.jd.com", name: "京东" }]，第二个参数是{ name: "京东" }。那么您需要以对象数组的形式返回第一个参数中的第三个元素，因为它包含第二个参数中定义的键 name，且对应的值"京东"相同


在介绍完整代码之前，我们先介绍下数组 Object.hasOwnProperty() 方法的具体用法： 

hasOwnProperty() 方法会返回一个布尔值，指示对象自身属性中是否具有指定的属性（也就是，是否有指定的键）。

语法:
obj.hasOwnProperty(prop)

参数:
prop 要检测的属性的 String 字符串形式表示的名称，或者 Symbol。

返回值:
用来判断某个对象是否含有指定的属性的布尔值 Boolean。

所有继承了 Object 的对象都会继承到 hasOwnProperty 方法。这个方法可以用来检测一个对象是否含有特定的自身属性；和 in 运算符不同，该方法会忽略掉那些从原型链上继承到的属性。


练习完整代码如下所示：

function findObjectInArrays( objs, obj ){
  var srcKeys = Object.keys(obj);

  return objs.filter(function(mobj) {
    for (var i = 0; i < srcKeys.length; i++) {
      if (
        !mobj.hasOwnProperty(srcKeys[i]) ||
        mobj[srcKeys[i]] !== obj[srcKeys[i]]
      ) {
        return false;
      }
    }
    return true;
  });
}

var sites = [{ domain: "www.icoderoad.comn", name: "路条编程" }, { domain: "www.tmall.com", name: null }, { domain: "www.jd.com", name: "京东" }];
console.log( findObjectInArrays(sites, {name: "京东" }) );
// => 0: {domain: "www.jd.com", name: "京东"}

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
