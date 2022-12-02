第一步.创建一个Proxy实例，该构造函数接收两个参数，第一个参数是被代理的对象，第二个参数是处理方法

~~~js
let proxy = new Proxy(object,{
    
})
~~~

第二步.在处理方法中设置“get”计算方法，该方法接收两个参数，第一个参数是被代理的对象，第二个参数是当前“get”读取的属性

~~~js
 get: function(target, propKey) {}
~~~

第三步.当第二个参数在第一个参数中时，“count“加1，否则减1

~~~js
 if(propKey in target) {
                count ++
            } else {
                count --
            }
~~~

最后一步：返回这个参数

~~~js
 return proxy
~~~

