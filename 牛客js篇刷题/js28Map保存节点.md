第一步.通过document.querySelector获取页面中“p”元素标签

~~~js
  let p = document.querySelector('p')
~~~

第二步.初始化Map实例保存“p”标签DOM节点和内容

~~~js
return new Map([[p,p.innerText]])
~~~

