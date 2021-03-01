---
id: 603c7d759975c65b84f5517b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用方括号访问属性名称
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用方括号访问属性名称

在关于对象的文章中，我们提到可以在方括号符号中用一个变量作为属性名来访问属性值。假设一个项目管理平台的的程序中使用了一个 project 对象，并且有一些程序逻辑会设置项目相关的属性，我们需要查询 project 对象来检查项目是否存在，我们可以这样写检查逻辑：

let mProject = getCurrentProject( projectName );
let name = projects[projectName];
上述代码会先获取 mProject 变量的值，并返回 projects 对象中以该值命名的属性对应的值，若没有以该值命名的属性则会返回 undefined。有时候对象的属性名在运行之前是不确定的，或者我们需要动态地访问对象的属性，这时方括号符号就会很有用。

下面的代码以中，我们已经定义了一个 getProjectNum 函数，它接受一个要获取项目名称作为输入参数。它要返回 projects  对象中以 projectName  的值命名的属性的值。只有有效的属性名会作为参数传入 getProjectNum ，此练习没有处理参数无效的情况。


let projects = {
  codeProjects: 38,
  buildProjects: 44,
  bugProjects: 12,
  releaseProjects: 22,
  testProjects: 10
};

function getProjectNum( projectName ) {
  let project = projects[ projectName ]
  return project;
}

console.log( getProjectNum("codeProjects") );
// => 38

console.log( getProjectNum("releaseProjects") );
// => 22

console.log( getProjectNum("testProjects") );
// => 10 

console.log( getProjectNum("errorProjects") );
// => undefined


以上代码定义了 getProjectNum 方法，根据传入项目名称获取项目数量， 前 3 个项目名称分别为 codeProjects、releaseProjects、testProjects 为存在的项目名称，分别返回对应的项目数，在控制台分别分出为 38、22、10、第 4 个项目名称为 projects 对象中不存在的项目名称，在控制台输出 undefined 。


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
