nginx_conf
==========

nginx.sleep.conf
--------------
实现: 接收用户请求后, 扔色子,决定是否处理用户的请求. 如果用户运气不佳, 让用户sleep一段时间

	$ curl http://127.0.0.1:8080/sleep
	sleep 4s & wake up

	$ curl http://127.0.0.1:8080/sleep
	sleep 1s & wake up

	$ curl http://127.0.0.1:8080/sleep
	sleep 3s & wake up

	$ curl http://127.0.0.1:8080/sleep
	sleep 3s & wake up

	$ curl http://127.0.0.1:8080/sleep
	sleep 1s & wake up

	$ curl http://127.0.0.1:8080/sleep
	Good luck

	$ curl http://127.0.0.1:8080/sleep
	sleep 5s & wake up

	$ curl http://127.0.0.1:8080/sleep
	sleep 6s & wake up

nginx.shared.conf
--------------
实现: 测试lua_shared_dict. 在线修改共享内存中的值

	$curl http://127.0.0.1:8080/getone
	取出1个, 剩余:4
	$curl http://127.0.0.1:8080/getone
	取出1个, 剩余:3
	$curl http://127.0.0.1:8080/getone
	取出1个, 剩余:2
	$curl http://127.0.0.1:8080/getone
	取出1个, 剩余:1
	$curl http://127.0.0.1:8080/getone
	取出1个, 剩余:0
	$curl http://127.0.0.1:8080/getone
	<html>
	<head><title>404 Not Found</title></head>
	<body bgcolor="white">
	<center><h1>404 Not Found</h1></center>
	<hr><center>ngx_openresty/1.4.3.3</center>
	</body>
	</html>
	$curl "http://127.0.0.1:8080/add?num=10"
	补充后,当前苹果数为:10
	$curl http://127.0.0.1:8080/getone
	取出1个, 剩余:9
	$


p.s. 

提交工程: 

git push origin master


