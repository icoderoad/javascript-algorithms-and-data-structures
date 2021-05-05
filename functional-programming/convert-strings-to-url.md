---
id: 6091f0ca1d6db1dda3ed1e52
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 应用函数式编程将字符串转换为 URL
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

应用函数式编程将字符串转换为 URL

最后几篇文章涵盖了许多符合函数式编程原则并在处理数组和字符串中非常有用的方法。我们还学习了强大的、可以将问题简化为更简单形式的 reduce 方法，从计算平均值到排序，任何数组操作都可以用它来实现。回顾一下，map 和filter 方法都是 reduce 的特殊实现。

现在是时候让我们把学到的所有知识结合起来解决一个工作中的实际问题了。

许多内容管理系统（CMS）为了让添加书签更简单，会将帖子的标题添加到 URL 上。举个例子，如果写了一篇标题为 "如何使用路条编程学习编程" 的帖子，URL 很可能会包含标题字符串的某种形式 (如：".../learn/如何使用路条编程学习编程")，如果您已经在路条编程网站上做过练习，您可能已经在 www.icoderoad.com 网站上注意到了这一点。

下面我们做个完整的练习，定义一个 titleToUrl 的方法，该方法包含一个参数 title，该方法将字符串 title 转换成带有连字符号(-)的 URL。您可以使用之前文章中介绍的任何方法，但不要用 replace 方法。
以下是该方法的详细要求：

title 参数为包含空格和标题大小写单词的字符串

方法返回字符串，单词之间的空格用连字符(-)替换

方法返回值应该是小写字母

方法返回值不应有任何空格

具体实现代码如下所示：

function titleToUrl( title ){
	
	return title
    .split(" ")
    .filter(substr => substr !== "")
    .join("-")
    .toLowerCase();

}

console.log( titleToUrl("hi kevin welcome to icoderoad") );
// => hi-kevin-welcome-to-icoderoad

经过以上代码的方法定义和执行结果可知，方法 titleToUrl 返回的字符串满足以上要求。
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
