---
id: 60485ab8606e22b988f5fec4
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 获取英文句子中最长单词的长度
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

获取英文句子中最长单词的长度

今天我们实现一个获取英文句子中最长单词长度的方法。 首先我们介绍两个方法的用法，一个是字符串的 split 方法，一个是数组的 sort 方法；

split() 方法使用指定的分隔符字符串将一个 String 对象分割成子字符串数组，以一个指定的分割字串来决定每个拆分的位置。 

语法：str.split([separator[, limit]])

参数：

separator 指定表示每个拆分应发生的点的字符串。separator 可以是一个字符串或正则表达式。 如果纯文本分隔符包含多个字符，则必须找到整个字符串来表示分割点。如果在str中省略或不出现分隔符，则返回的数组包含一个由整个字符串组成的元素。如果分隔符为空字符串，则将str原字符串中每个字符的数组形式返回。

limit  一个整数，限定返回的分割片段数量。当提供此参数时，split 方法会在指定分隔符的每次出现时分割该字符串，但在限制条目已放入数组时停止。如果在达到指定限制之前达到字符串的末尾，它可能仍然包含少于限制的条目。新数组中不返回剩下的文本。

返回值：

返回源字符串以分隔符出现位置分隔而成的一个 Array 


sort() 方法用原地算法对数组的元素进行排序，并返回数组。默认排序顺序是在将元素转换为字符串，然后比较它们的 UTF-16 代码单元值序列时构建的。

语法：

arr.sort([compareFunction])

参数：

compareFunction 可选，用来指定按某种顺序进行排列的函数。如果省略，元素按照转换为的字符串的各个字符的 Unicode 位点进行排序。

firstEl 第一个用于比较的元素。

secondEl  第二个用于比较的元素。

返回值： 排序后的数组。请注意，数组已原地排序，并且不进行复制。

为了实现我们的要求，我们需要定义一个方法 getLenLongestWord， 参数为 str，为我们要查的的英文句子，该方法的返回值应该是一个数字。具体实现步骤如下所示：

1、将句子进行分割，并把每个单词存入到数组中

2、分别获取每个单词的长度，并存入到另一个数组中
 
3、对存储单词长度的数组按从大到小顺序排序
 
4、返回新数组第一个元素值


具体实现代码如下所示：

function getLenLongestWord(str) {
  
  var arr = str.split(" ");
  var a = [];
  for (var i in arr) {
    a.push(arr[i].length);
  }
   
  return a.sort(function (a, b) {
    return b-a;
  })[0];
}

下面是两个美到窒息的英文句子，我们以它们做为测试的句子。

Two things fill the mind with ever new and increasing admiration and reverence - the starry heavens above me and the moral law within me.有两件事我愈是思考，心中就愈充满惊叹与敬畏 - 我头顶上的璀璨星空与我内心的道德准则。
—— 康德

console.log( getLenLongestWord('Two things fill the mind with ever new and increasing admiration and reverence - the starry heavens above me and the moral law within me.') );
// => 10

Let life be beautiful like summer flowers and death like autumn leaves. 
生如夏花之绚烂，死如秋叶之静美。
—— 泰戈尔

console.log( getLenLongestWord('Let life be beautiful like summer flowers and death like autumn leaves.') );
// => 9

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
