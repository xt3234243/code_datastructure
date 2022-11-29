要求返回一个长度为参数值并且每一项值都为参数值的数组。

大概是这个效果：假设输入3

返回结果为[3,3,3]

第一步：创建新的number数组 参数是多少，长度就是多少

~~~js
let arr = new Array(number);
~~~

第二步：去填充数组里的value,长度是多少，每个值就是多少

~~~js
 let newArr = arr.fill(number);
~~~

最后返回这个新的数组

~~~js
return newArr;
~~~

