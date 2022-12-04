## 获取两个节点的共同父节点，可以包含本身(最简单方法 递归)

~~~js
function commonParentNode(oNode1, oNode2) {
let parent1 = oNode1.parentNode;
let parent2 = oNode2.parentNode;
if(parent1 === parent2){
return parent1
}else{
commonParentNode(parent1,parent2)
}
}
~~~

