# onload 的几种方式

## <body onload="init()"> 

* 代码

```html
<body onload="init()">
	
</body>
```

```javascript
var init = funciton(){
	//....
}
```

## 事件方式

* 代码

```javascritpt
document.addEventListener('DOMContentLoaded',function(){
	//...
})
```

## window.onload

* 代码

```javascript
window.onload = function(){
	//...
}
```