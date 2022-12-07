遍历数组，arguments只是类数组，并没有数组的一些方法

进行相加

~~~js
function useArguments() {
    let sum = 0;
    for(let i = 0; i < arguments.length; i++){
        sum += arguments[i];
    }
    return sum;
}
~~~

