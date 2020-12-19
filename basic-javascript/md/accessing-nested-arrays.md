---
id: 5fddd189cde0a2591c03773e
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 访问嵌套数组中对象及根据键值更新对象属性值
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
访问嵌套数组中对象及根据键值更新对象属性值。

我们在前面的文章中介绍过在对象中可以嵌套对象和数组。与访问嵌套对象一样，用中括号操作符同样可以访问嵌套数组。

下面是如何访问嵌套数组的例子：

var pets = [
  {
    animalType: "cat",
    names: [
      "龙二",
      "卡卡西",
      "雄霸"
    ]
  },
  {
    animalType: "dog",
    names: [
      "艾拉",
      "索尔",
      "八神"
    ]
  }
];

console.log(pets[0].names[1]); // => 卡卡西
console.log(pets[1].names[0]); // => 艾拉

操作复杂对象的文章中我们介绍过 JSON 对象，我们这次还以 JSON 对象为例，给定一个 JSON 对象，用来表示喜爱音乐的列表。每首歌曲都有几个属性和一个唯一的 id 号作为键值。并非所有歌曲都有完整的信息。

写一个函数，根据传入的歌曲 id（如 689 ）、属性如 "artist" 或 "title" 如 "踏山河"，来修改音乐列表中歌曲的数据。

提示：通过变量访问对象的属性时，应使用中括号。

var musicAlbums = {
    901: {
      title: '踏山河1',
      artist: '是七叔呢',
      release_year: 2020
    },
    189: {
      title: '燕无歇',
      artist: '是七叔呢',
      release_year: 2020
    },
    321: {
      title: '茫',
      artist: '李润祺',
      release_year: 2020
    },
    689: {
      title: '醒不来的梦',
      artist: '回小仙',
      release_year: 2020
    }
  };

function updateMusic(id, key, val) {
  var music = musicAlbums[id];
  music[key] = val;
  musicAlbums[id] = music ;
}

updateMusic( 901, 'title', '踏山河');
console.log( musicAlbums);

以上代码定义了一个音乐列表对象 musicAlbums，定义函数 updateMusic ，根据 id 获取列表中的歌曲对象，根据给定的 key 和 val ,更新对象的属性值。
 执行语句 updateMusic( 901, 'title', '踏山河'); ，修改指定 id 对象的属性值。根据控制台的输出结果，可以查看到更新后的音乐列表中 id 为 901 的对象 title 值为 踏山河， 已经不是之前的 踏山河1 了。

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
