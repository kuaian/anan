07.26 15:53
从数组中删除虚值，随机替换
var mixedArr = [0, “blue”, “”, NaN, 9, true, undefined, “white”, false];
var trueArr = mixedArr.filter(Boolean);
console.log(trueArr); // returns [“blue”, 9, true, “white”]




9.从数组中删除虚值

在 JS 中，虚值有 false, 0，''， null, NaN, undefined。咱们可以 .filter() 方法来过滤这些虚值。


10  js   随机替换

var colors = ['a','b','c','d','e','f','g'];


var x = colors[(Math.floor(Math.random() * (colors.length)))]



var  y=Math.floor(Math.random()*33+1); 



document.getElementById(x).innerHTML=y; 


11   php  数组里删除虚值

php  数组也可以从数组里删除虚值，

php  数组 定胆随机自动回收，都需要删除虚

值0。




