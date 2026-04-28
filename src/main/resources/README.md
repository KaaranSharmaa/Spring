Ioc->means that inversion of control like programmer don't think about object  they have to also so that they can think about bussiness 
IOC CONTANIER-> WILL HAVE THE OBJ AND WILL BE HANDEL BY spring frame work
dependency injection mean that you have to obj inject krte hai spring k through
spring is there on top pf it spring boot is there
spring is a modular frame work which means it will ask you what you want to add
mvn spring-boot:run
any obj create and manage by spring is called beans

Which Spring module is used for integrating ORM tools like Hibernate?
Spring orm

What annotation is used in Spring to automatically inject dependencies?
@autowired

Which feature of Spring is used to separate cross-cutting concerns like logging?
AOP

ApplicationContext context And calling bean
ApplicationContext context = new ClassPathXmlApplicationContext("spring.xml");
Alien obj = (Alien) context.getBean("alien");  
in xml 
<!-- Bean Definitions -->
 <bean id="alien1" class="com.telusko.Alien">
 </bean>
 <bean id="alien2" class="com.telusko.Alien">
 </bean>
 <bean id="lap" class="com.telusko.Laptop">
 </bean>
</beans>

