Two key principles :
Dependency Injection  -constructor, setter
Inversion of  control

Spring autowires dependency at run time. This allows developers to write loosely coupled code
Metadata
XML and Java annotations

Web, business and data layer  - collaboration of objects across these layers is called dependencies

Tight coupling

Loose coupling

Spring is a dependency injection framework that promotes loose coupling

Development timeline:
Java 5 - > Spring 3.0 - > Springboot 1.0
Java 8 - > Spring 5.0 - > Springboot 2.0
Java 17 - > Spring 6.0 -> Springboot 3.0

Terminology
objects  - instance of a class - > beans (Managed by Spring)
dependency

Annotations:
@Component

Autowiring - the process of identifying a dependency, and then populating the dependency is called autowiring

Example : (Inversion of control)
Vehicle -----------> Engine
creates

Vehicle <----------- Engine
Injection(done by Spring framework)


Ioc Container (There are two implementations)
---------------
Bean factory  - legacy
Application context - new (Enterprise solutions)


Spring
- modules
- Data Access Integration
- JDBC
- ORM (Hibernate, JPA)
- Transactions
- JMS
- OXM
- Web Mvc
- Web
- Servlet
- Struts
- AOP
- Aspects
- Instrumentation
- Spring Core Container
- Core
- Beans
- Context
- Expression Language
- Test
- Junit
- TestNg

Spring projects for Enterprise solutions
- Spring Boot
- Spring Cloud
- Spring Data
- Spring Integration
- Spring Batch
- Spring Security
- Spring Mobile
- Spring Android

Decoupling components : 
 - use interfaces to make your code loosely coupled
 - inject dependencies through a constructor

 Beans (The instances or objects that spring manages)
Dependencies
Location of the beans

@Component (which are the beans)
@Autowired (manage dependency between them)
@ComponentScan (Location of the beans)

@SpringBootApplication = @Configuration + @EnableAutoConfiguration + @ComponentScan

steps when we run the application :
Loading source class = Spring tries find anything with @Component annotation
Identified Candidate component class
Creating shared instance of singleton bean


Autowiring by type @Primary when there are more than one components to inject dependency
Autowiring by name - reference name should be the same as the dependency class
if you apply both the approaches at the same time, @Primary takes precendence
