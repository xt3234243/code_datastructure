题目的意思就是获取文件扩展名

例如：1.html   获取html

​	 1.js  获取js

> ​	相当于python里的切片
>
> slice（start,end）
>
> 从 start 索引开始提取数组元素，直至 end 索引（包括 start，但不包括 end）

第一步：通过lastIndexOf方法获取最后一个"."符号的位置

~~~js
let index = filename.lastIndexOf('.')
~~~

第二步：通过slice截取index（点）（包括）之后的字符串

其次 获取index后，使用slice获取index之后的字符，即'.text' 。要注意 filename可能为空，至少我做题的时候 题目没说是否为空，所以要用三目来判断。

~~~js
   return index !== -1 ? filename.slice(index) : ' '
~~~

