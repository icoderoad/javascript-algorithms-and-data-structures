---
id: 601799d491155b6cab8aca55
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 通过正则编写用户名限制规则
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 正则表达 测试方法、字符串匹配、查找、替换、检查混合字符和捕获组模式等。通过学习 正则表达式 这一系列文章，您将会逐步掌握 正则表达式 基础相关的知识。

通过正则编写用户名限制规则

用户名在互联网上随处可见。它们是用户在自己喜欢的网站上的唯一身份。我们在编写用户注册程序时经常要对用户名进行规则限制，需要检索数据库中是否存在此用户名。以下是用户在注册用户时用户名必须遵守的一些规则。

1) 用户名只能是数字字母字符。

2) 用户名中的数字必须在最后，且数字可以有零个或多个。

3) 用户名字母可以是小写字母和大写字母。

4) 用户名长度必须至少为两个字符。两位用户名只能使用字母。

我们根据上面的规则做个练习，代码示例如下所示：

let userName = "happyCode";
let userCheck = /^[a-z]([0-9]{2,}|[a-z]+\d*)$/i;
let result = userCheck.test(userName);
console.log( result );
// => true

上面代码中正则表达式详细说明：

^ - 输入开始
[a-z] - 第一个字符是字母
[0-9]{2,0} - 以两个或更多数字结尾
| - 或
[a-z]+ - 后面有一个或多个字母
\d* - 以零或更多数字结尾
$ - 输入结束
i - 忽略输入的大小写

我们先设置了一个用户名赋值给变量 userName, 然后编写正则表达式赋值给变量 userCheck， 通过正则表达式 test 方法进行规则验证，将验证结果赋值给变量 result ，并将结果在控制台输出，输出结果为 true，经过测试得出，正则表达式满足上面 4 条用户名规则。

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
