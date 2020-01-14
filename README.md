# Spring-Annotation-Example

    Spring framework implements and promotes the principle of control inversion (IOC) or dependency injection (DI) and is in fact     an IOC container.
    Traditionally, Spring allows a developer to manage bean dependencies by using XML-based configuration.
    There is an alternative way to define beans and their dependencies. This method is a Java-based configuration.
    Unlike the XML approach, Java-based configuration allows you to manage bean components programmatically. That’s why Spring annotations were introduced.
    
    
  1.  @Configuration annotation in spring:

@Configuration annotation in spring is use to eliminate the Spring Bean Configuration file means without Spring Bean 
configuration file we can get the dependency in spring framework.

@Configuration annotation in spring was introduced in Spring 3.0 and It provides an alternative to XML-based configuration.

@Configuration annotation indicates that a class declares one or more @Bean methods and may be 
processed by the Spring container to generate bean definitions and service requests for those beans at run time.


2.@Bean annotation in spring:

@Bean annotation in spring is used to declare a single bean , the @Bean annotation returns an
 object that spring should register as bean in application context.

@Bean annotation in spring is alternate of <bean id=”beanid” class=”class_name”> 
tag of spring Bean Configuration file.

@Bean annotation in spring will be used along with @Configuration annotation .

3.@Value annotation in spring is use to pass 
	 * default value  for the Pojo class property 
	 * and @Value annotation in spring is an alternate 
	 * of <propety> tag of Spring Bean Configuration file. 
  
  4.@Required:
  if we want to mandate some fields to be mandatory to be injected then we have to use @Required annotation with setter method.
  5.@Scope annotation in spring

@Scope annotation in spring is use to change the scope of bean life cycle  within the Spring IoC Container as we know  by default Scope of bean is singleton but if want to change the scope of bean then we can use @Scope annotation in spring Framework.

6.Spring @Autowired Annotation

Spring @Autowired Annotation is use to manage the dependency automatic. If we annotated any dependent class by using @Autowired annotation then Spring IoC container is able to find dependency and manage dependency implicitly.
We can manage dependency in spring framework by using autowire attribute in spring XML configuration file using ref attribute or by using @Autowired annotation.
We can use @Autowired annotation on variables  or methods or on constructor or on Attribute.

7.@Qualifier annotation in spring
@Qualifier to be used along @AutoWired
@Qualifier annotation in spring is use to resolve the spring bean ambiguity problem. When two or more than two similar beans having same class are declared in bean configuration.
If  two similar beans having same class are declared in bean configuration file then Spring IoC Container will not able to understand which bean should autowired and Spring IoC Container will ends up with some exception  org.springframework.beans.factory.BeanCreationException with message No unique bean of type.

Spring Stereotype Annotations

Spring Stereotype Annotations is used to categorized clearly application layers and We can write easily an AOP pointcut using Spring Stereotype Annotations that targets.

There are four Spring Stereotype Annotations are available.
1.@Component generic stereotype for any Spring-managed component
 2.@Repository stereotype for persistence layer                  
3.@Service   stereotype for service layer                      
 4.@Controller| stereotype for presentation layer (spring-mvc) 
    
