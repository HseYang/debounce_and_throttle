节流(debounce)和防抖(throttle)的工具

使用很简单 需要配置简单的参数 调用即可

## 2019.10.26：
	- 1.0.0
	- 节流和防抖功能
	
### 使用方法:
	
   > <script type="text/javascript">
		// 具体方法可看index.html文件 有demo演示
   
		var debounce = function(func, wait = 1000, immediate = true, throttle = false) {
	   		// ......
		})
	   
		var test1 = debounce(function() {
			console.log("防抖 点击第一次执行")
		}, 1000)

		var test2 = debounce(function() {
			console.log("防抖 点击最后一次执行")
		}, 1000, false)

		var test3 = debounce(function() {
			console.log("节流 每次都“延迟”执行")
		}, 1000, false, true)
			
		var test4 = debounce(function() {
			console.log("节流 每次都“及时”执行")
		}, 1000, true, true)
	   
   </script>