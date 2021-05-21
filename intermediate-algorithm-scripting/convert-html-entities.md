---
id: 60a4a21b2c03a5bfa33b3019
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 将传入字符串中HTML标签进行转义处理

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您中级算法脚本相关的范围内数字求和、区分两个数组、搜索与替换、集合排序、求斐波那契数组中的奇数之和、二进制转换及构造对像类等相关算法问题。

将传入字符串中HTML标签进行转义处理

本次练习我们需要写一个函数 convertHTMLTag 。该方法接收一个参数，该方法将传入字符串中的 HTML 标签中的&、<、>、"（双引号）和'（单引号）进行转义后返回。

在介绍完整代码之前，我们先介绍下字符串 split 方法和数组 map 方法的具体用法： 

split() 方法使用指定的分隔符字符串将一个String对象分割成子字符串数组，以一个指定的分割字串来决定每个拆分的位置。 

语法：
str.split([separator[, limit]])

注意：如果使用空字符串(“)作为分隔符，则字符串不是在每个用户感知的字符(图形素集群)之间，也不是在每个Unicode字符(代码点)之间，而是在每个UTF-16代码单元之间。这会摧毁代理对。还请参见how do you get a string to a character array in javascript

参数：
separator 指定表示每个拆分应发生的点的字符串。separator 可以是一个字符串或正则表达式。 如果纯文本分隔符包含多个字符，则必须找到整个字符串来表示分割点。如果在str中省略或不出现分隔符，则返回的数组包含一个由整个字符串组成的元素。如果分隔符为空字符串，则将str原字符串中每个字符的数组形式返回。

limit 一个整数，限定返回的分割片段数量。当提供此参数时，split 方法会在指定分隔符的每次出现时分割该字符串，但在限制条目已放入数组时停止。如果在达到指定限制之前达到字符串的末尾，它可能仍然包含少于限制的条目。新数组中不返回剩下的文本。

返回值：
返回源字符串以分隔符出现位置分隔而成的一个 Array 

map() 方法创建一个新数组，其结果是该数组中的每个元素是调用一次提供的函数后的返回值。

语法：
var new_array = arr.map(function callback(currentValue[, index[, array]]) {
 // Return element for new_array 
}[, thisArg])

参数：
  callback
    生成新数组元素的函数，使用三个参数：
      currentValue
        callback 数组中正在处理的当前元素。
      index可选
        callback 数组中正在处理的当前元素的索引。
      array可选
        map 方法调用的数组。
  thisArg可选
    执行 callback 函数时值被用作this。

返回值：
一个由原数组每个元素执行回调函数的结果组成的新数组。

练习完整代码如下所示：

function convertHTMLTag(str) {
  const htmlEntities = {
    "&": "&amp;",
    "<": "&lt;",
    ">": "&gt;",
    '"': "&quot;",
    "'": "&apos;"
  };
  
  return str
    .split("")
    .map(entity => htmlEntities[entity] || entity)
    .join("");

  return str;
}

console.log( convertHTMLTag("icoderoad < develop < javascript") );
// => icoderoad &lt; develop &lt; javascript 

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
