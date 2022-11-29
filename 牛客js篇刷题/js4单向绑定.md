题目要求，当改变输入框中的值时，id为“span”的“span”标签内容同步修改

第一步：获取“input”，span的元素

~~~js
let a = document.getElementById("input");
let b = document.getElementById("span");

~~~

第二步：当input内容改变时，用onchange方法，span里的内容也改变，将input里的内容赋给span

~~~js
a.onchange = function(){
  //把a改变的值赋值给b  
  //右边赋值给左边，
  //左边一般是不变的 甚至是常量类，这也是经开发的一种规范
  b.innerHTML = a.value;
}
~~~

