第一步.返回的结果为调用fn之后的结果

~~~js
return fn（）
~~~

第二步.fn的调用参数为calllt的第一个参数之后的全部参数

~~~js
...[...arguments].slice(1)
~~~

