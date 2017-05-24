###JavaScript入坑(一)

___

[JavaScript 参考手册](http://www.w3school.com.cn/jsref/index.asp)

[完整的 HTML DOM 对象参考手册（包含实例）](http://www.w3school.com.cn/jsref/index.asp)

[github](https://github.com/huanghehg/JavaScript.git)
___

<strong>`document.write();`内嵌`html`语句，写入`html`输出</strong>

```
document.write("<h1>This is a heading</h1>");
document.write("<h2>This is a paragraph</h2>");
```

<strong>`alert(), onclick()`</strong>

```
<button type="button" onclick="alert('测试')">戳这里</button>
```
<strong>`getElementById `根据`id`获取控件，改变内容</strong>

```
<p id="test1">改变之前的数据</p>

<script type="text/javascript">
function changeTest() {
	x = document.getElementById('test1');
	x.innerHTML = "改变之后的数据";
}
</script>

<button onclick=changeTest()>戳这里改变</button>
```

<strong>`image`</strong>

```
<script type="text/javascript">
	function changeImage() {
		image = document.getElementById('tes1image');
		if (image.src.match("ermilio")) {
			image.src = "./resources/img/mew_interlaced.png"
		}else {
			image.src = "./resources/img/ermilio.png"
		}
		
	}
</script>

<img id="tes1image" src="./resources/img/ermilio.png" onclick="changeImage()">
```