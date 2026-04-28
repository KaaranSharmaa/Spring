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
**********************************************************************************************************
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
**********************************************************************************************************
Types of Bean Scopes:
1. Singleton (Default Scope):
○ In the Singleton scope, only one instance of the bean is created, even
if there are multiple references to it.
○ Every time we retrieve the bean from the Spring container, we will get
the same instance.
2. Prototype:
○ In the Prototype scope, a new object is created each time when we call
the getBean() method.
○ Each reference will point to a distinct instance of the bean.
3. Request (for Spring Web):
○ In the Request scope, a new bean instance is created for every HTTP
request. This scope is available in web applications.
4. Session (for Spring Web):
○ In the Session scope, a new bean instance is created for every HTTP
session. This scope is specific to web applications.
Singleton:
<bean id="alien1" class="com.telusko.Alien" />
Or
<bean id="alien1" class="com.telusko.Alien" scope="singleton" />
Prototype
<bean id="alien1" class="com.telusko.Alien" scope="prototype" />
**********************************************************************************************************
Setter injection 
in this we can pass the vlaue of setter in xml rather thn giving in the main class

<bean id="alien1" class="com.telusko.Alien" >
<property name="age" value="21"> </property>//age is the variable deifine in the setter
</bean>
**********************************************************************************************************



