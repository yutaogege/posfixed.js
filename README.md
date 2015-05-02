<div class="wrap">
	<h2 id="a1">说明</h2>
	<p>Posfixed 能够让网页的导航或表头等固定在顶部或底部，让用户更方便的操作或查看信息，淘宝网、易迅网等电子商务网站常常用到这种效果。除了导航和表头，也可以固定其他内容，比如广告、返回顶部等等，同时 Posfixed 也可以作为 IE6 不支持 fixed 的一个解决方案。</p>
	<p class="highlight">本演示中，导航和右下的“返回顶部”使用了 Posfixed 插件，请注意查看效果。</p>
	
	<h2 id="a2">使用</h2>
	<h3>引入文件</h3>
	<pre>&lt;script src="js/jquery.min.js"&gt;&lt;/script&gt;
&lt;script src="js/posfixed.js"&gt;&lt;/script&gt;</pre>
	
	<h3>HTML</h3>
	<pre>&lt;div id="example1"&gt;
&lt;/div&gt;</pre>
	
	<h3>JavaScript</h3>
	<pre>$(document).ready(function(){
	$("#example1").posfixed({
		distance:0,
		pos:"top",
		type:"while",
		hide:false
	});             
});</pre>
	
	<h2 id="a3">参数</h2>
	<table>
		<thead>
			<tr>
				<th width="65">参数</th><th width="60">类型</th><th>说明</th><th width="60">默认值</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>direction</td><td>字符串</td><td>方向，相对于顶部（top）或底部（bottom）固定</td><td>top</td>
			</tr>
			<tr>
				<td>type</td><td>字符串</td><td>固定的方式，可选 while 或 always，while 为滚动条滚动到 distance 的数值时固定；always 为一直固定</td><td>while</td>
			</tr>
			<tr>
				<td>hide</td><td>布尔值</td><td>是否自动隐藏固定的对象</td><td>false</td>
			</tr>
			<tr>
				<td>distance</td><td>整数</td><td>离顶部或底部的数值</td><td>0</td>
			</tr>
			<tr>
				<td>tag</td><td>对象</td><td>导航到一个元素</td><td>null</td>
			</tr>
		</tbody>
	</table>

	<h2 id="a4">兼容</h2>
	<p>Posfixed 兼容以下浏览器：</p>
    <ul class="list">
    	<li>Firefox 2+</li>
    	<li>Internet Explorer 6+</li>
    	<li>Safari 2+</li>
    	<li>Opera 9+</li>
    	<li>Chrome</li>
    </ul>
</div>
