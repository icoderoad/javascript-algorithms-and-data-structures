---
id: 6033412563f6e1f27373b062
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 slice() 拷贝数组元素
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 slice() 拷贝数组元素

今天我们要介绍 slice() 方法。slice() 方法并不修改数组，而是复制或者说提取给定数量的元素到一个新数组里，而调用方法的数组则保持不变。

slice() 方法返回一个新的数组对象，这一对象是一个由 begin 和 end 决定的原数组的浅拷贝（包括 begin，不包括 end ）。原始数组不会被改变。

语法：arr.slice([begin[, end]])

参数：

begin 可选，提取起始处的索引（从 0 开始），从该索引开始提取原数组元素。
如果该参数为负数，则表示从原数组中的倒数第几个元素开始提取，slice(-2) 表示提取原数组中的倒数第二个元素到最后一个元素（包含最后一个元素）。
如果省略 begin，则 slice 从索引 0 开始。
如果 begin 超出原数组的索引范围，则会返回空数组。

end 可选，提取终止处的索引（从 0 开始），在该索引处结束提取原数组元素。slice 会提取原数组中索引从 begin 到 end 的所有元素（包含 begin，但不包含 end）。
slice(1,4) 会提取原数组中从第二个元素开始一直到第四个元素的所有元素 （索引为 1, 2, 3的元素）。
如果该参数为负数， 则它表示在原数组中的倒数第几个元素结束抽取。 slice(-2,-1) 表示抽取了原数组中的倒数第二个元素到最后一个元素（不包含最后一个元素，也就是只有倒数第二个元素）。
如果 end 被省略，则 slice 会一直提取到原数组末尾。
如果 end 大于数组的长度，slice 也会一直提取到原数组末尾。

返回值：一个含有被提取元素的新数组。

slice() 只接受 2 个输入参数—第一个是开始提取元素的位置（索引），第二个是结束提取元素的位置（索引）。slice 方法会提取直到截止索引的元素，但被提取的元素不包括截止索引对应的元素。


请看以下例子：

let welcomeMsgs = ['您好', '菜鸟008', '欢迎', '访问', '路条', '编程！'];

let msgArr = welcomeMsgs.slice(1, 3);
console.log( msgArr );
// =>  ["菜鸟008", "欢迎"]

console.log( welcomeMsgs );
// => (6) ["您好", "菜鸟008", "欢迎", "访问", "路条", "编程！"]

以上代码定义了一个字符串数组 welcomeMsgs， 该数组包含 6 个元素 ，定义提取开始位置为 1，结束位置为 3，执行 slice 方法进行数据提取，将提取数据赋值给变量 msgArr。在控制台打印提取数组及原数组，根据控制台输出结果可知，提取数组数据为 “["菜鸟008", "欢迎"]”，从开始到结束提取位置，不包含结束位置元素，原数组数据没有变化。


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
