1������eureka����
	windows��ָ�� java -Xms64m -Xmx64m -jar eureka.jar
	linux��ָ��(����־) nohup java -Xms64m -Xmx64m -jar eureka.jar eureka.out 2>&1 & 
		 ��(����־) nohup java -Xms64m -Xmx64m -jar eureka.jar /dev/null 2>&1 & 

2������˽��Լ��ķ���idע�ᵽeureka�����÷�ʽΪ spring: application: name: xxx

3���ͻ������������ϼ���ע�� @EnableFeignClients 

4���ͻ��˱�дopenFeign�ӿ��࣬�ڽӿ��ϼ���ע�� @FeignClient("xxx") ���� xxx ����Ӧ��2���е� xxx  


http://101.200.76.13:8888/summary/feign-server.git
http://101.200.76.13:8888/summary/feign-client.git