---
id: 5ffed1bc808cd6d65edfb387
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 export 语句从模块导出函数， 使用 import 语句复用导出函数
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用 export 语句从模块导出函数， 使用 import 语句复用导出函数。

前面文章中我们介绍了定义函数和对象的相应方法。如果我们想使用之前定义好的函数，我们应该如何操作呢？假如我们需要一些数学运算中常用的方法，类似两数的加减乘除运算。以加法为例，我们在文件 math_utils.js 中定义一个加法函数，将加法运算存储在变量 add 中，该函数接受两个数字做为参数返回它们的和。如果想在其它不同的 JavaScript 文件里使用这个函数，需要 export 语句导出此方法，代码示例如下：

export const add = (x, y) => {
  return x + y;
}

上面是导出单个函数的常用方法，也可以通过下面的方式导出：

const add = (x, y) => {
  return x + y;
}

export { add };

导出变量和函数后，就可以在其它文件里导入使用从而避免了代码冗余。重复第一个例子的代码可以导出多个对象或函数，在第二个例子里面的导出语句中可以添加使用逗号“，”分隔的多个值导出多项，代码示例如下所示：

export { add, subtract };


我们可以使用 import 语句导入文件或模块导出的相应方法。以导出上面 math_utils.js 文件里导出了 add 方法为例，下面看一下如何在其它的文件导入 add 方法。

import { add } from './math_utils.js';

在这里，import 语句会在 math_utils.js 里找到 add 函数，只导入这个函数，忽略导出的其它函数。上面代码中 ，from 语句后面的 ./ 告诉程序在当前文件的相同目录寻找 math_utils.js 文件。用这种方式导入时，相对路径（./）和文件扩展名（.js）都是必需的。

可以在导入语句里导入多个函数，代码示例如下所示：

import { add, subtract } from './math_utils.js';

我们还可以用 import 语句从文件 math_utils.js 中导入所有的内容。下面是一个从相同目录下的 "math_utils.js" 文件中导入所有函数的例子：

import * as mathUtils from "./math_utils.js";

上面的 import 语句会创建一个 mathUtils 对象。这只是一个变量名，可以随便命名。对象包含 math_utils.js 文件里所有导出的函数，可以像访问对象的属性那样访问里面的函数。下面是使用导入的 add 和 subtract 函数的示例：

mathUtils.add(2,3);
mathUtils.subtract(5,3);

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
