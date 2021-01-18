---
id: 60002418a43af1be4a07962c
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 创建一个默认导出和导入一个默认的导出
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
创建一个默认导出和导入一个默认的导出。

在介绍 export 语法的课程中，我们学习了导出的相关语法。通过此语法可以在其他文件中引用一些函数或者变量。

我们还需要了解另外一种被称为默认导出的 export 语法。在需要导出的文件中只有一个值需要导出的时候，通常会使用这种语法。它也常常用于给文件或者模块创建返回值。

我们继续以算术运算中的加法为例，下面是一个简单的默认导出 export default 例子：

//有函数名 add 的函数
export default function add(x, y) {
  return x + y;
}

// 匿名函数
export default function(x, y) {
  return x + y;
}

注意：当使用 export default 去声明一个文件或者模块的返回值时，在每个文件或者模块中应当只默认导出一个值。特别要注意的是 export deafult 语句 需要与 var，let 和const一起使用。

上面默认导出的函数，我们如果想在其他文件中使用的话，需要使用 import 语句来导入默认的导出函数或变量。

下面示例是导入 math_utils.js 文件默认导出的 add 函数，详细语句如下所示：

import add from "./math_utils.js";

这个语法只有一处与前面文章介绍不同的地方，就是被导入的 add 函数并没有放在花括号 {} 中。与导出值的方法不同，导入默认导出的写法仅仅只是简单的将变量名写在 import 之后即可。


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
