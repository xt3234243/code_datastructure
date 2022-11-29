补充：返回随机数的公式

random()会返回一个浮点型伪随机数字，范围[0, 1)

- 返回一个两数之间的 随机数 ,范围在[start, end)

  >Math.random()*(end - start)

  ​


- 返回一个两数之间的 整数 ,范围在[start, end)

  > `// floor向下取整`
  >
  > Math.floor(Math.random()*(end - start))


- 返回一个两数之间的 整数 ,范围在[start, end]




第一步：定义一个数组，用来存随机数

~~~js
 const res = []
~~~

第二步：产生随机数的代码

~~~js
 let num = Math.floor(Math.random()*(end-start+1))+start
~~~

第三步：如果数组里没有重复的元素，就push一下

~~~js
  if (!res.includes(num)) {
        res.push(num)
      }
~~~

最后一步：返回这个数组

~~~js
  return res
~~~

