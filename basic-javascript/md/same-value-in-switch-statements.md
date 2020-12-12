---
id: 5fd404c064fe98c1ac16ba2d
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 switch 语句通过不同条件值设置相同结果及替换多个 if 条件语句
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用 switch 语句通过不同条件值设置相同结果及替换多个 if 条件语句。

在使用 switch 语句时，如果你忘了给 switch 语句的每一条 case 条件添加 break 语句 ，那么直到遇见第一个 break 语句为止，后续的 case 会一直执行。如果你想为多个不同的条件值设置相同的结果，可以通过不写 break 语句的方式实现，以一个判断是否为工作日的函数为例，如果为周一至周五为工作日，否则为休息日。示例代码如下所示：

function ifWorkDay( day ) {
  var result = "";
  switch( day ) {
    case 1:
    case 2:
    case 3:
    case 4:
    case 5:
      result = "工作日";
      break;
    case 6:
    case 0:
      result = "周末";
      break;
    default:
       result = "非法参数";
  }
  return result;
}

console.log( ifWorkDay(0) ); // => 周末
console.log( ifWorkDay(5) ); // => 工作日
console.log( ifWorkDay(8) ); // => 非法参数

通过 0、5、8 不同的参数值调用函数 ifWorkDay ， 并且在控制台将结果输出，控制台分别输出 周末、工作日和非法参数。

如果你有多个条件需要判断，switch 语句写起来会比多个串联的 if/if else 语句容易些，还拿判断是否为工作日的函数为例，定义函数名为 ifWorkDay2，代码如下所示:

function ifWorkDay2( day ) {
  var result = "";
  if (day === 1 || day === 2 || day === 3 || day === 4 || day === 5 ) {
    result = "工作日";
  } else if ( day === 0  || day === 6 ) {
     result = "周末";
  } else {
    result = "非法参数";
  }
  return result;
}

console.log( ifWorkDay2(0) ); // => 周末
console.log( ifWorkDay2(5) ); // => 工作日
console.log( ifWorkDay2(8) ); // => 非法参数

通过在控制台调用两个函数 ifWorkDay 和 ifWorkDay2，大家可以通过比较下控制台输出结果，虽然结果一致，但是 switch 语句的代码比 if/if else 语句简洁些。如果有类似的条件判断，建议使用 switch 语句替换多个串联的 if/if else 语句。  

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
