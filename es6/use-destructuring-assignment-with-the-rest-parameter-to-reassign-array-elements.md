---
id: 5ff6b0716036b0fde01100d6
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用解构赋值配合 rest 操作符来重新分配数组元素及参数化解构
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用解构赋值配合 rest 操作符来重新分配数组元素及参数化解构。

在解构数组的某些情况下，我们可能希望将剩下的元素放进另一个数组里面。

以下代码的结果与使用 Array.prototype.slice() 相同：

const [numA, numB, ...numArr] = [8, 12, 41, 32, 69, 91];
console.log(numA, numB); // => 8 12
console.log(numArr); // => [41, 32, 69, 91]


变量 numA 与 numB 分别获取了数组的前两个元素的值。之后，因为 rest 操作符的存在，numArr 获取了原数组剩余的元素的值，并构成了一个新的数组。 rest 操作只能对数组列表最后的元素起作用。这意味着您不能使用 rest 操作符来截取原数组中间元素的子数组。

下面我们做个练习，使用解构赋值以及 rest 操作符来进行一个 Array.prototype.slice 相同的操作。使得 langArr 是原数组 devLangs 除开前两个元素的子数组。


const devLangs = ['java', 'javascript', 'c', 'c++', 'python', 'html', 'css', 'php', 'nodejs', 'csharp'];
function removeFourLang(list) {
  "use strict";
  const [lang1, lang2, lang3, lang4, ...arr] = list;
  return arr;
}
const langArr = removeFourLang(devLangs);
console.log(langArr); // => ["python", "html", "css", "php", "nodejs", "csharp"]
console.log(devLangs); // => ["java", "javascript", "c", "c++", "python", "html", "css", "php", "nodejs", "csharp"]

在某些情况下，也可以在函数的参数里直接解构对象。

请看以下代码：

const profileUpdate = (profileData) => {
  const { name, age, nationality, location } = profileData;
}

上面的操作解构了传给函数的对象。这样的操作也可以直接在参数里完成：

const profileUpdate = ({ name, age, nationality, location }) => {
 
}

这样的操作去除了多余的代码，使代码更加整洁。 这样做还有个额外的好处就是函数不需要再去操作整个对象，而仅仅是操作复制到函数作用域内部的参数。

下面对 half 的参数进行解构赋值，使得仅仅将 max与 min 的值传进函数。
const statsObj = {
  max: 56.78,
  standard_deviation: 4.34,
  median: 34.54,
  mode: 23.87,
  min: -0.75,
  average: 35.85
};

修改前代码：
const half = (stats) => (stats.max + stats.min) / 2.0;
console.log( half(statsObj) ); // => 28.015
修改后代码：
const half2 = ({ max, min }) => (max + min) / 2.0;
console.log( half2( statsObj )); // => 28.015 
经过比较，以上两种方式定义的函数，控制台输出结果都为 28.015， 下面的代码更简洁，逻辑更清楚。

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
