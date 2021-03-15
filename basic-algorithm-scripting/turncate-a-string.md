---
id: 604bfce02736d3312bd46a89
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过三种方法按指定长度截断字符串的方法
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

通过三种方法按指定长度截断字符串的方法

今天我们介绍通过三种方法按指定长度截断字符串的方法。如果字符串长于给定的最大字符串长度，则截断该字符串。返回带有 ... 结尾的截断字符串。 我们在介绍具体实现方法之前，先熟悉下字符串的 substring() 方法、substr() 方法和 slice() 方法。

substring() 方法返回一个字符串在开始索引到结束索引之间的一个子集, 或从开始索引直到字符串的末尾的一个子集。

语法：

str.substring(indexStart[, indexEnd])

参数：

indexStart  需要截取的第一个字符的索引，该索引位置的字符作为返回的字符串的首字母。

indexEnd  可选。一个 0 到字符串长度之间的整数，以该数字为索引的字符不包含在截取的字符串内。

返回值：包含给定字符串的指定部分的新字符串。

如果 indexStart 等于 indexEnd，substring 返回一个空字符串。

如果省略 indexEnd，substring 提取字符一直到字符串末尾。

如果任一参数小于 0 或为 NaN，则被当作 0。

如果任一参数大于 stringName.length，则被当作 stringName.length。

如果 indexStart 大于 indexEnd，则 substring 的执行效果就像两个参数调换了一样。

substr() 方法返回一个字符串中从指定位置开始到指定字符数的字符。

语法：

str.substr(start[, length])

参数：

start   开始提取字符的位置。如果为负值，则被看作 strLength + start，其中 strLength 为字符串的长度（例如，如果 start 为 -3，则被看作 strLength + (-3)）。

length 可选。提取的字符数。

start 是一个字符的索引。首字符的索引为 0，最后一个字符的索引为字符串的长度减去 1。substr 从 start 位置开始提取字符，提取 length 个字符（或直到字符串的末尾）。

如果 start 为正值，且大于或等于字符串的长度，则 substr 返回一个空字符串。

如果 start 为负值，则 substr 把它作为从字符串末尾开始的一个字符索引。如果 start 为负值且 abs(start) 大于字符串的长度，则 substr 使用 0 作为开始提取的索引。注意负的 start 参数不被 Microsoft JScript 所支持。

如果 length 为 0 或负值，则 substr 返回一个空字符串。如果忽略 length，则 substr 提取字符，直到字符串末尾。

slice() 方法返回一个新的数组对象，这一对象是一个由 begin 和 end 决定的原数组的浅拷贝（包括 begin，不包括end）。原始数组不会被改变。

语法：

arr.slice([begin[, end]])

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

返回值：

一个含有被提取元素的新数组。

实现步骤如下所示：

1、 判断字符串长度是否大于最大长度, 如果大于，进行字符串截取操作，否则直接返回字符串

2、如果大于最大长度，截取最大长度字符串赋值给一个变量

3、在截取后的字符串变量结尾增加 ...

4、返回处理后的字符串

第一种方法：使用 substring() 方法进行截取

let defStr = '当你面对蓝天的时候，你要学会翱翔长空；当你面对高山的时候，你要学会坚韧不拔；当你面对长河的时候，你要学会奔流不息。人，决不可驻足停留。';
function truncateStr(str, num) {
  if( str.length > num ){

    str = str.substr(0, num) ;
    str += '...'; 
  }
  return str;
}

console.log( truncateStr(defStr, 10) );
// => 当你面对蓝天的时候，...


第二种方法：使用 substr() 方法进行截取

function truncateStr2(str, num) {
  if( str.length > num ){
    str = str.substr(0, num) ;
    str += '...'; 
  }
  return str;
}
console.log( truncateStr2(defStr, 15) );
// => 当你面对蓝天的时候，你要学会翱...


第三种方法：使用 slice() 方法进行截取

function truncateStr3(str, num) {
  if( str.length > num ){
    str = str.slice(0, num) ;
    str += '...'; 
  }
  return str;
}
console.log( truncateStr3(defStr, 21) );
// => 当你面对蓝天的时候，你要学会翱翔长空；当你...


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
