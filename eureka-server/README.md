1.eureka 服务器，在springcloud 中充当服务发现注册中心，于使用dubbo Rpc 方式搭建的微服务平台，其作用类似于zookeeper

2.简单的创建eureka 服务 ，只需要在启动类中使用@EnableEurekaServer 注解就可以

3.当搭建高可用的注册服务器时，可以将服务器的eureka.serviceUrl.defaultZone=指向对方服务器
同时，将eureka client 中的eureka.serviceUrl.defaultZone=添加多个注册中心的地址
