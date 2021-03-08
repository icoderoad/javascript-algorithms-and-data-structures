---
id: 6045d396e688eb90d0889b9f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 用递减的 while 循环反转字符串
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

用递减的 while 循环反转字符串

今天我们练习一个反转字符串的功能。我们需要需要先将字符串转换为数组，然后将数组转换为对应的字符串。我们定义一个方法为 reverseString， 参数为 str ，方法返回值为反转后的字符串。

function reverseString(str) {
   
    var strArr = [];
 	var len = str.length;
 	var index = len -1;
    console.log( '字符串长度为：' + len);
    var i=0;
    while( index>=0 ){ 
    	i++;
    	strArr.push(str[ index ]); 
    	console.log('第' + i + '次迭代:index = ' + index + ', 数组 strArr 为' + strArr );
        index--;
    }
  
    return strArr.join(""); 
}

let returnStr = reverseString("icoderoad");
console.log( returnStr );

以上代码执行步骤如下所示：
步骤1：创建一个空数组, 数组变量为 strArr
步骤2：创建 while 循环并执行循环语句
循环的执行条件为 index >=0

字符串长度为：9
第1次迭代:index = 8, 数组 strArr 为d
第2次迭代:index = 7, 数组 strArr 为d,a
第3次迭代:index = 6, 数组 strArr 为d,a,o
第4次迭代:index = 5, 数组 strArr 为d,a,o,r
第5次迭代:index = 4, 数组 strArr 为d,a,o,r,e
第6次迭代:index = 3, 数组 strArr 为d,a,o,r,e,d
第7次迭代:index = 2, 数组 strArr 为d,a,o,r,e,d,o
第8次迭代:index = 1, 数组 strArr 为d,a,o,r,e,d,o,c
第9次迭代:index = 0, 数组 strArr 为d,a,o,r,e,d,o,c,i
循环结束，返回反转后字符串：daoredoci

步骤3：返回反转字符串 daoredoci 赋值给变量 returnStr
步骤4：控制输出返回后的字符串 daoredoci

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
