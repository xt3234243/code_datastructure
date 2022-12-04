call()、bind()、apply()的用法，改变this的指向，区别在于
f.call(obj, arg1, arg2...),
f.bind(obj, arg1, arg2,...)(),
f.apply(obj, [arg1, arg2, .])

大多数情况下用call 

apply的用法

~~~js
function bindThis(f, oTarget) {
 return function() {
     return f.apply(oTarget, arguments)
 }
}
~~~
bind的用法

~~~js
function bindThis(f, oTarget) {
 return f.bind(oTarget)
}
~~~
call的用法
~~~js
function bindThis(f, oTarget) {
 return function() {
     return f.call(oTarget, ...arguments)
 }
}
~~~

