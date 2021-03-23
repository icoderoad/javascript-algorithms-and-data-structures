---
id: 60572837f75d6eacdc2e2407
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将数组拆分为指定数量的子数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

将数组拆分为指定数量的子数组

今天我们介绍将数组拆分为指定数量的子数组方法。在介绍具体方法之前，我们先介绍下数组的 push() 方法。

push() 方法将一个或多个元素添加到数组的末尾，并返回该数组的新长度。

语法：

arr.push(element1, ..., elementN)

参数：

elementN 被添加到数组末尾的元素。

返回值：

当调用该方法时，新的 length 属性值将被返回。

实现步骤如下所示：

1、初始化一个数组 chunks

2、使用 for 循环遍历要拆分的数组

3、每当索引 ％ size 为 0 时，添加另一个子数组，然后将该项目推到最后一个子数组

4、 将元素添加至子数组

5、返回初始的数组 chunks


具体代码如下所示：

function chunkArrayInGroups(arr, size) {

   var chunks = [];
  
  for(var i = 0; i < arr.length; i++) {    
    if(i % size === 0) {
      chunks.push([]);
    }
    
    chunks[chunks.length - 1].push(arr[i]);
  }
  
  return chunks;

}

console.log( chunkArrayInGroups(["路条", "百度", "阿里", "腾讯"], 2) );
// => (2) [Array(2), Array(2)]

console.log( chunkArrayInGroups(["icoderoad", "baidu", "ali", "qq"], 2) );
// => (2) [Array(2), Array(2)]

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
