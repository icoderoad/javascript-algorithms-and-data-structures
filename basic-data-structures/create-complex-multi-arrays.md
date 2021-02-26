---
id: 603886741571baf2906c8213
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 创建复杂的多维数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

创建复杂的多维数组

到目前为止，您已经学到很多关于数组的知识了！但这些只是一个开始，您将在接下来的文章中学习到更多与数组相关的知识。但在继续去学习对象（Objects）之前，让我们再花一点时间看一看，数组怎样能够变得比之前的练习中更复杂一点。

数组的一个强大的特性是，它可以包含其他数组，甚至完全由其他数组组成。我们已经在之前文章的练习中看到了包含数组的数组，但它还算是比较简单的。数组中的数组还可以在包含其他数组，数组中是可以嵌套任意层数组的。数组从而可以被用来实现非常复杂的叫做多维或嵌套数组的数据结构。请看如下代码示例：

let mArrs = [ // 顶层，或第 1 层——最外层的数组
  ['level2'], // 数组中的数组，第 2 层
  [
    ['level3'], ['level3'] // 第 3 层嵌套的两个数组
  ],
  [
    [
      ['level4'], ['level4'] // 第 4 层嵌套的两个数组
    ],
    [
      [
        ['level5'] // 第 5 层嵌套的一个数组
      ]
    ]
  ]
];

虽然这个例子看起来错综复杂，但这样复杂的数组并不算罕见，尤其是在处理大量数据的时候。 但我们仍能简单地用方括号符号来访问到嵌套得最深的数组：

console.log(mArrs[2][1][0][0][0]);
// => level5

既然我们知道数据在哪里，我们同样也能修改它：

mArrs[2][1][0][0][0] = '修改后的 level5';

console.log(mArrs[2][1][0][0][0]);
// => 修改后的 level5


下面我们来做个完整的练习，我们定义了一个 demoArrs 数组变量。使用字符串（string）、数使字（number）或者布尔值（boolean）作为数组的数据元素，使得 demoArrs 刚好有 5 层数组嵌套（记住，最外层的数组是第 1 层）。请在第 3 层的数组中包含字符串' 路条'，在第 4 层的数组中包含字符串'编程'，在第 5 层的数组中包含字符串 '欢迎您！'。 然后将多维数组中的 “路条”、“编程”、“欢迎您！” 欢迎信息取出，赋值给变量 welcomeMsg, 在控制台输出相应的欢迎信息。

let demoArrs = [
  '第一层',                    /* demoArrs[0]             */
  ['第二层'],                  /* demoArrs[1][0]          */
  [['第三层','路条']],         /* demoArrs[2][0][0]       */
  [[['第四层','编程']]],       /* demoArrs[3][0][0][0]    */
  [[[['第五层','欢迎您！']]]]  /* demoArrs[4][0][0][0][0] */
];

let welcomeMsg = demoArrs[2][0][1] + demoArrs[3][0][0][1] + demoArrs[4][0][0][0][1];
console.log( welcomeMsg );
// => 路条编程欢迎您！

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
