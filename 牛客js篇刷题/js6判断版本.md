

**join()** 方法将一个数组（或一个[类数组对象](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Indexed_collections#%E4%BD%BF%E7%94%A8%E7%B1%BB%E6%95%B0%E7%BB%84%E5%AF%B9%E8%B1%A1_array-like_objects)）的所有元素连接成一个字符串并返回这个字符串，用逗号或指定的分隔符字符串分隔。如果数组只有一个元素，那么将返回该元素而不使用分隔符

第一步：去除新旧版本号中的“.”，用split方法将其变成数组[1,1,1],然后再用join方法返回成一个字符串“111”

~~~js
oldVersion.split('.').join('')
newVersion.split('.').join('')
~~~

第二步：将新旧版本号的字符串转换为数字

~~~js
parseInt（）
~~~

最后一步：进行比较

~~~js
   return newversion > oldversion
~~~

