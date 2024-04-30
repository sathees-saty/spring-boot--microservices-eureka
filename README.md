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
# Steps 2 create Item-Catalog microservice and register with EurekaServer
* File -> Spring starter project -> EurekaServer
* 1.	Spring Boot Actuator
* 2.	Eureka Discovery Client
* 3.	Spring Data JPA
* 4.	H2 Database
* 5.	Rest Repositories
* 6.	Spring Web
* 7.	Spring boot Dev tools
* 8.	Lombok
* Project created 
* Add @EnableDiscoveryClient to Application class
* And update Application class as coded
* Go to application.properties 
* Added server.port = 8088
* Create application-cloud.properties file and update as mentioned in the github
* Select project:
* Maven clean
* Maven build -success 
* Goals: spring-boot:run
* You will get pop up from IDE. You need to accept then only the services are registered and up other wise services are down in http://localhost:8761/
* ![image](https://github.com/sathees-saty/spring-boot--microservices-eureka/assets/65384711/eb03630e-2121-43a3-a6e1-5f5a090b61f8)
*  open http://localhost:8088/items and http://localhost:8088/items/1
* ![image](https://github.com/sathees-saty/spring-boot--microservices-eureka/assets/65384711/7101d4eb-027a-41fc-869a-fcd6acf796d3)
* ![image](https://github.com/sathees-saty/spring-boot--microservices-eureka/assets/65384711/2b975bea-a750-4971-9cba-a765e63e99a9)
* You can test the same in postman also
# Steps 3 Create with project name eurekaclient as Spring Starter project as microservice and register with EurekaServer
* Add dependencies
* 1.	Spring Boot Actuator
* 2.	Eureka Discovery Client
* 3.	Spring Data JPA
* 4.	H2 Database
* 5.	Rest Repositories
* 6.	Spring Web
* 7.	Spring boot Dev tools
* 8.	Lombok
* 9.	thymeleaf
* Update Application class file with annontations
* update application.properties 


