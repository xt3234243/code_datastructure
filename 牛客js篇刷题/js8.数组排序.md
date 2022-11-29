第一步.

接收一个数组参数，函数内创建一个空字符串用于保存HTML模板，遍历数组项创建HTML模板并且拼接在空字符串之后，最终将字符串中的HTML模板值给ul的innerTHML

创建一个渲染函数，每次升序或降序后都渲染一遍

先定义一个空的字符串

遍历每一个元素

写入ul里面

~~~js
const _listRendering = arr => {
    var str = ''
    arr.forEach(element => {
        str += `<li>${element.name}</li>`
    })
    ul.innerHTML = str
}
~~~

第二步：运用sort方法，数字排序升序用a-b，数字排序降序用b-a，给”销量升序“和”销量降序“绑定点击事件，分别按照"升序"、"降序"排列数组再调用渲染函数

~~~
upbtn.onclick = function () {
    var upArr = cups.sort(function (a, b) {
        return a.sales - b.sales
    })
    _listRendering(upArr)
}
downbtn.onclick = function () {
    var downArr = cups.sort(function (a, b) {
        return b.sales - a.sales
    })
    _listRendering(downArr)
}
~~~



