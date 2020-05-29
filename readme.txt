1、启动eureka服务
	windows下指令 java -Xms64m -Xmx64m -jar eureka.jar
	linux下指令(有日志) nohup java -Xms64m -Xmx64m -jar eureka.jar eureka.out 2>&1 & 
		 或(无日志) nohup java -Xms64m -Xmx64m -jar eureka.jar /dev/null 2>&1 & 

2、服务端将自己的服务id注册到eureka，配置方式为 spring: application: name: xxx

3、客户端在启动类上加入注解 @EnableFeignClients 

4、客户端编写openFeign接口类，在接口上加入注解 @FeignClient("xxx") 其中 xxx 即对应第2步中的 xxx  


http://101.200.76.13:8888/summary/feign-server.git
http://101.200.76.13:8888/summary/feign-client.git