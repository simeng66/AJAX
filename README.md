# 解析json
- eval(危险！！！)

			var jsonData='{"staff":[{"name":"小红","age":17},      
			  {"name":"小白","age":7},{"name":"小花","age":11},     
			  {"name":"红红","age":11}]}';
			var jsonObg=eval('('+jsonData+')');
			alert(jsonObg.staff[0].name);
            
-  JSON.parse 

			var jsonData='{"staff":[{"name":"小红","age":17},     
			  {"name":"小白","age":7},{"name":"小花","age":11},     
			  {"name":"红红","age":11}]}';
			var jsonObg=JSON.parse(jsonData);
			alert(jsonObg.staff[0].name);

# Json校验工具--JSONLint

# Json跨域
json出于安全的考虑，不允许跨域调用其它页面的对象，解决方法如下：

-  通过在同域名的服务器端创建一个代理（后端解决方式）
-  JSONP可用于解决主流浏览器的跨域数据访问的问题(只能处理get）
-  处理跨域方式XHR2
