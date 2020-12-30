---
layout: default
title:  "Coding Post"
description: An example post which shows code rendering.
date:   2019-05-23 21:03:36 +0530
categories: Javascript NodeJS
---
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse

```javascript
const express = require('express')
const app = express()
 
app.get('/', function (req, res) {
  res.send('Hello World')
})
 
app.listen(3000)
```

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquam qui voluptatem excepturi nemo similique atque sapiente aperiam, dolorum deleniti! Esse quam perferendis temporibus nemo at molestias necessitatibus tenetur cupiditate sapiente. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nihil et voluptatibus non labore officiis assumenda, distinctio perspiciatis blanditiis nesciunt rerum molestias impedit fugiat nulla qui libero minima quasi! Libero, iure.



弱引用的作用在于解决强引用所带来的对象之间在存活时间上的耦合关系。弱引用最常见的用处是在集合类中，尤其在哈希表中。哈希表的接口允许使用任何Java对象作为键来使用。当一个键值对被放入到哈希表中之后，哈希表对象本身就有了对这些键和值对象的引用。如果这种引用是强引用的话，那么只要哈希表对象本身还存活，其中所包含的键和值对象是不会被回收的。如果某个存活时间很长的哈希表中包含的键值对很多，最终就有可能消耗掉JVM中全部的内存。



通过软引用重获方法实现Java对象的高速缓存



- 虚引用是最弱的引用
- 虚引用对对象而言是无感知的，对象有虚引用跟没有是完全一样的
- 虚引用不会影响对象的生命周期
- 虚引用可以用来做为对象是否存活的监控

使用虚引用的目的就是为了得知对象被GC的时机，所以可以利用虚引用来进行销毁前的一些操作，比如说资源释放等。这个虚引用对于对象而言完全是无感知的，有没有完全一样，但是对于虚引用的使用者而言，就像是待观察的对象的把脉线，可以通过它来观察对象是否已经被回收，从而进行相应的处理。

事实上，虚引用有一个很重要的用途就是用来做堆外内存的释放，DirectByteBuffer就是通过虚引用来实现堆外内存的释放的。

**0**|**1****小结**

```scss
body {
	font-family: 'Nunito Sans', sans-serif;
	line-height: 1.5em;
	margin: 0;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
}
```
Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquam rerum, ratione impedit necessitatibus facere soluta odio repellat asperiores neque! Sunt iusto quia suscipit amet inventore eum, vel molestiae reiciendis alias.