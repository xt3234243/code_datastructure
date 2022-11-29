该题运用splice方法

splice(start)
splice(start, deleteCount)
splice(start, deleteCount, item1)
splice(start, deleteCount, item1, item2, itemN)

第一步.通过concat方法完全拷贝一份新的数组

~~~js
 let newarray = array.concat()
~~~

第二步，运用splice方法，将参数所对应的索引值删掉

~~~js
newarray.splice(index,1)
~~~

最后返回一个新的数组

~~~js
return newarray
~~~

