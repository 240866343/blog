---
title: 闭包现象
---
- 在一个函数内部，有权访问另一个函数中的变量（并且能够随时访问）！
- 尽量不要去看长篇大论关于闭包的解释，很容易把自己绕晕。看一些很容易理解的例子帮助你更好的理解闭包才是最好的！

### 闭包 一 : 访问变量局限性大，不能自由访问。

```
function show1() {
         var a = 10;
        function show2() {
           console.log(a)
         }
  show2();
}
show1();

```
### 闭包 二 : 可以自由访问。
```
function show() {
         var a = 10;
          return:  function() {
           console.log(a)
         }
}
show()();

```

### 常见闭包一般出现在DOM节点操作中，看下面典型例子！

```
为每一个li添加点击事件，并且弹出他所在ul中的位置。

<ul id="list">
    <li>aaa</li>
    <li>aaa</li>
    <li>aaa</li>
</ul>

var  lis=document.getElementById("list").getElementsByTagName("li");
for(var i=0;i<lis.length;i++){
   lis[i]._index=i;//为每个li添加一个属性并且保存他的所在的位置。
   lis[i].onclick=function(){
          alert(i)//无论你点那个，弹出的都是3!
         alert(this._index);//可以弹出相应的位置!this指你事件触发者.即你点击的 li !
    }
}
```
---

### 其实闭包现象随处可见，虽然他很容易出问题且不容易调试
### 所以你也可以去试试啦，听着很牛逼的闭包，其实也没什么，哈哈哈哈。。。。