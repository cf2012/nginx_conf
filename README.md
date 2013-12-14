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



p.s. 

提交工程: 

git push origin master
