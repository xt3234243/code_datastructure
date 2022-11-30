![66977287648](assets/1669772876482.png)

every的用法

**every()** 方法测试一个数组内的所有元素是否都能通过某个指定函数的测试。它返回一个布尔值。

第一步.判断两个set对象的长度是否一致，不一致返回false

~~~js
   if (s1.size !== s2.size) {
        return false
    }
~~~

第二步.通过ES6[...]扩展字符将set对象的伪数组转换为数组，再调用every进而判断该数组中的每一项是否存在于另一个set对象中

~~~js
  return [...s1].every(i => s2.has(i))
~~~

