#自定义右键菜单插件
 方法
* face：右键点击区域，接受class名。必须
* menu:弹出菜单容器，接受class名。必须
* huidiao:回调函数，用于菜单选项的js定义，不必须，
 <br />实例化示例：
```javascript
  var shili = new rightKeyMenu({
    face:"js-face",//点击区域
    menu:"js-menu",//菜单
    huidiao:function() {//回调函数
    var i = 0,
    lis = document.querySelectorAll(".js-menu li");
    for(i; i < lis.length; i++){
      lis[i].onclick = function() {
        console.log(this.innerHTML);
        document.querySelector(".menu").style.display = "none";//点击后隐藏菜单
      }
    }
  }
})
```
##兼容性:ie9+
## (示例demo)[https://lijinwen1994.github.io/ife_2017/自定义右键菜单插件/]
