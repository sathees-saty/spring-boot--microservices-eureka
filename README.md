# spring-boot--microservices-eureka

# Steps 1 create EurekaServer
* File -> Spring starter project -> EurekaServer
* Add dependency -> Eureka Server
* Project created
* Update application.properties 
* server.port = 8767
* eureka.client.register-with-eureka=false
* Important: Open Application class and add @EnableEurekaServer – it will enable other applications to communicate
* Run Application class as Springboot application
* Open browser http://localhost:8761/
* EurekaServer started running , refer below screenshot. But no instances are registered
* ![image](https://github.com/sathees-saty/spring-boot--microservices-eureka/assets/65384711/4cb85329-d055-4084-8176-9f97a14ff86a)

