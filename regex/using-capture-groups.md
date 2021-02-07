---
id: 601d0a9fe491e4cecc80d653
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用捕获组重用模式及搜索和替换
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

使用捕获组重用模式及搜索和替换

实际工作中，一些您所搜寻的匹配模式会在字符串中出现多次，手动重复该正则表达式太浪费了。有一种更好的方法可以指定何时在字符串中会有多个重复的子字符串。

可以使用捕获组搜寻重复的子字符串。括号 ( 和 ) 可以用来匹配重复的子字符串。只需要把重复匹配模式的正则表达式放在括号中即可。

要指定重复字符串将出现的位置，可以使用反斜杠（\）后接一个数字。这个数字从 1 开始，随着您使用的每个捕获组的增加而增加。这里有一个示例，\1 可以匹配第一个组。

下面的示例匹配任意两个被空格分割的单词：

let repeatStr = "ha ha ha song"; // 啦啦操
let repeatRegex = /(\w+)\s\1/;
let result = repeatRegex.test(repeatStr); 
console.log( result );
// => true

result = repeatStr.match(repeatRegex);
console.log( result );
// => ["ha ha", "ha", index: 0, input: "ha ha ha song", groups: undefined]

以上代码我们使用正则表达式应字符的速记元字符 \w 进行重复字符设置， \s 表示任意空格符, \1 表示匹配第一个组。设置重复字符串变量 repeatStr 为英文歌 啦啦操 的名称，然后使用 test 和 match 方法进行测试及匹配，最后将结果输出至控制台，控制台最终输出结果为 true 和 ["ha ha", "ha", index: 0, input: "ha ha ha song", groups: undefined]。

在正则表达式中，搜索功能是很有用的。但是，当搜索同时也执行更改（或替换）匹配文本的操作时，搜索功能就会显得更加强大。

可以使用字符串上 .replace() 方法来搜索并替换字符串中的文本。.replace() 方法的输入首先是想要搜索的正则表达式匹配模式，第二个参数是用于替换匹配的字符串或用于执行某些操作的函数。

let welcomeMsg = "路条编程(www.ioderoad.com) 欢迎您！";
let testRegex = /ioder/;
let result = welcomeMsg.replace(testRegex, "icode");
console.log( result );
// => 路条编程(www.icodeoad.com) 欢迎您！

以上代码使用 .replace() 搜索并替换匹配的字符串，我们将路条编程域名故意写错为 www.ioderoad.com， 将正则表达式 /ioder/ 赋值给变量 testRegex 用于搜索，然后使用字符串变量 welcomeMsg 的 replace 方法进行搜索替换，替换字符串为 icode， 并将结果输出到控制台，控制台输出结果为 ”路条编程(www.icodeoad.com) 欢迎您！“

您还可以使用美元符号（$）访问替换字符串中的捕获组。

let result = "Welcome Icoderoad".replace(/(\w+)\s(\w+)/, '$2 $1');
console.log( result );
// => Icoderoad Welcome


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
