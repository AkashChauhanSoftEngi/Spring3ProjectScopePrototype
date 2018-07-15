# Spring3ProjectScopePrototype

* Spring 3 + IOC (Core Container) + Scope(Prototype), Example
* As scope is prototype so in this case if you call getBean method multiple times,
  container sends only multiple object references to the JVM and would create multiple objects
* Used BeanFactory Interface, and used XmlBeanFactory Implementation class
* XmlBeanFactory is called driver class to run IOC container from main method.
* Used applicationContext.xml for defining beans
* Spring requires Spring JAR/Libraries and JDK Libraries to run an Spring based application 
* We need a driver class [XmlBeanFactory] to run Spring container[IOC], which implements BeanFactory Interface

```XML
 	<bean id="studentbean" class="com.java.spring.Student" scope ="prototype">  
    		<property name="name" value="Vimal Jaiswal"></property>  
  	</bean>
```

```java
	ClassPathResource resource = new ClassPathResource("applicationContext.xml");
 	BeanFactory factory = new XmlBeanFactory(resource);
```

> **###1. Technologies**
* Spring 3.0.1.RELEASE

