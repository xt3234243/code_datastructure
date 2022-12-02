第一步.通过[...prototypes]获取从第二个参数开始往后的所有参数

~~~js
 let privatePrototype = prototypes
~~~

第二步.创建一个Proxy实例并且返回，该构造函数接收两个参数，第一个参数是被代理的对象，第二个参数是处理方法

~~~js
  return new Proxy(object, {}）
~~~

第三步.在处理方法中设置“get”计算方法，该方法接收两个参数，第一个参数是被代理的对象，第二个参数是当前“get”读取的属性

~~~js
 get(object, prototype) {}
~~~

第四步.` 当获取某个实例属性时，如果这个属性在[...prototypes]数组中，则返回”noright“

~~~js
if(privatePrototype.includes(prototype)) return 'noright'
~~~

最后

~~~js
return object[prototype]
~~~

