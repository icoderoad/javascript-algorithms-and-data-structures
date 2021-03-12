---
id: 6049adacc3158e6605a55747
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 检查字符串是否以给定的目标字符串结束
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

检查字符串是否以给定的目标字符串结束

今天我们练习一个字符串是否以目标字符串结束的检测方法。我们通过两种方式实现检测。
第一种方法为字符串自带的 endsWith() 方法，第二种方法通过字符串的 length() 方法和  substr 方法实现。

endsWith() 方法用来判断当前字符串是否是以另外一个给定的子字符串“结尾”的，根据判断结果返回 true 或 false。

语法：

str.endsWith(searchString[, length])

参数：

searchString	要搜索的子字符串。
length 可选，作为 str 的长度。默认值为 str.length。

返回值：

如果传入的子字符串在搜索字符串的末尾则返回true；否则将返回 false。


substr() 方法返回一个字符串中从指定位置开始到指定字符数的字符。

语法：

str.substr(start[, length])

参数：

start 	开始提取字符的位置。如果为负值，则被看作 strLength + start，其中 strLength 为字符串的长度（例如，如果 start 为 -3，则被看作 strLength + (-3)）。
length 	可选。提取的字符数


length  该属性返回字符串中字符编码单元的数量。JavaScript 使用 UTF-16 编码，该编码使用一个 16 比特的编码单元来表示大部分常见的字符，使用两个代码单元表示不常用的字符。因此 length 返回值可能与字符串中实际的字符数量不相同。空字符串的 length 为 0。静态属性 String.length 返回 1。

我们定义两个方法，checkStringEnding 和 checkStringEnding2 ，分别都包含两个参数， 第一个参数 str 为要检测的字符串，第二个参数 target 为目标字符串，检测字符串是否以 target 字符串结尾。

function checkStringEnding(str, target) {
  if(str.endsWith(target)){	
		return true;
	}else{	
		return false;
	}
}

let result = checkStringEnding('生如夏花之绚烂，死如秋叶之静美', '静美');
console.log( result );
// => true

result = checkStringEnding('生如夏花之绚烂，死如秋叶之静美', '静-美');
console.log( result );
// => false

function checkStringEnding2(str, target) {
  let index = str.length-target.length;
  if(str.substr(index,target.length)==target)
    return true;
  else 
    return false;
}

result = checkStringEnding2('生如夏花之绚烂，死如秋叶之静美', '静美');
console.log( result );
// => true

result = checkStringEnding2('生如夏花之绚烂，死如秋叶之静美', '静-美');
console.log( result );
// => false

以上代码实现中，第一种方法直接使用字符串自带的 endsWith 方法，比较简单，我们不作解释。 第二种方法实现逻辑如下：

1、通过两个字符串的长度之差，获取目标字符串结束位置

2、调用字符串 substr 取子串方法，获取检测字符串从指定位置 index 开始的结束子串

3、比较检测字符串子串与目标字符串是否相等

4、返回比较结果




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
