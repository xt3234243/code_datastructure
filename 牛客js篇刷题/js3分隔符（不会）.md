第一步：先把数字转化成字符串

~~~js
 let str = number.toString();
~~~

第二步：用正则匹配

~~~js
 return  str.replace(/(\d)(?=(?:\d{3})+$)/g, '$1,');
~~~

