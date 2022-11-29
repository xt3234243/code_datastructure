方法一：直接打印输出即可  br代表换行

~~~js
           triangle.innerHTML=`
                *<br>**<br>***<br>

`
~~~

方法二：循环遍历,外层循环控制行，内层循环控制内容的变化

第一步：先控制行，输出一行弄一个换行符

~~~js
var str =' '
for(let i =1;i<=3;i++){
    
    str+=“<br/>”
}
~~~

第二步：控制内容变化 （规律是1、2、3）

~~~js
for(let j=1;j<=i;j++){
    str+='*'
    
}
~~~

第三步：把内容赋给str

~~~js
triangle.innerHTML=str
~~~

