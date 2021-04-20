---
id: 607b74544445b1f451506440
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 了解使用命令式编程的危害

---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您函数式编程的原则、编程术语、避免函数中的外部依赖、重构全局变量、使用 map、filter 方法从数组中提取数据、使用 slice、 concat、reduce 方法来解决复杂问题等。

了解使用命令式编程的危害

函数式编程是一种好习惯，它能让代码管理更简单，不受隐藏 bug 影响。在我们开始函数式编程之前，为了更好的突显可能遇到的问题，我们先看看命令式编程。

类似在英语中，命令式时态用于给出命令，编程中的命令式是给计算机一组语句来执行任务。

这些语句通常会改变程序的状态，例如更新全局变量，典型的例子就是写一个 for 循环，它给出了迭代数组索引的精确方向。

相反，函数式编程是声明式编程的一种形式，通过调用方法或函数来告诉计算机要做什么。

JavaScript 提供了许多处理常见任务的方法，所以您无需写出计算机应如何执行它们。例如，您可以用 map 函数替代上面提到的 for 循环来处理数组迭代。这有助于避免语义错误，如调试章节介绍的"Off By One Errors"。

考虑这样的场景：您正在浏览器中浏览网页，并想操作打开的标签。下面我们来试试用面向对象的思路来描述这种情景。

窗口对象由选项卡组成，通常会打开多个窗口。窗口对象中每个打开网站的标题都保存在一个数组中。在对浏览器进行了如打开新标签、合并窗口、关闭标签之类的操作后，您需要输出所有打开的标签。关掉的标签将从数组中删除，新打开的标签（为简单起见）则添加到数组的末尾。

下面代码显示了此功能的实现，其中包含 tabOpen()，tabClose()，和 join() 函数。tabs 数组是窗口对象的一部分用于储存打开页面的名称。

在控制台中运行以下代码。它使用了有副作用的方法，导致输出错误。打开标签的最终列表应该是 ['QQ', '微信', '淘宝', '百度', '阿里', '央视频', '微博', '人民网','路条编程', '新标签'] 但输出会略有不同。


var Window = function(tabs) {
  this.tabs = tabs; 
};


Window.prototype.join = function (otherWindow) {
  this.tabs = this.tabs.concat(otherWindow.tabs);
  return this;
};

Window.prototype.tabOpen = function (tab) {
  this.tabs.push('new tab'); 
  return this;
};

Window.prototype.tabClose = function (index) {

  var tabsBeforeIndex = this.tabs.splice(0, index);
  var tabsAfterIndex = this.tabs.splice(1);
  this.tabs = tabsBeforeIndex.concat(tabsAfterIndex); 
  
  return this;
 };

var workWindow = new Window(['百度', '阿里', '央视频', '路条编程']); 
var socialWindow = new Window(['微博', '人民网']);
var videoWindow = new Window(['QQ', '微信', '淘宝', '百度']);

var finalTabs = socialWindow
  .tabOpen() 
  .join(videoWindow.tabClose(2))
  .join(workWindow.tabClose(1).tabOpen());
console.log(finalTabs.tabs);
// => (10) ["微博", "人民网", "new tab", "QQ", "微信", "百度", "百度", "央视频", "路条编程", "new tab"]

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
