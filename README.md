# Spring  

## IoC (Inversion of Control) 控制反转  

* 是一种思想，把对象的创建，赋值，管理工作都交给代码之外的容器实现，也就是对象的创建是由其他的外部资源完成。

* 控制：创建对象，对象的属性赋值，对象之间的管理关系

* 反转：把开发人员创建管理对象的权限转移给代码之外的容器实现

* 容器：是一个软件，一个框架(spring)

* java中创建对象的方式

	1. 构造方法 new()

	2. 反射

	3. 序列化

	4. 克隆

	5. IoC：容器创建对象  



### IoC的体现

servlet  

1. 创建继承类 HttpServlet

2. 在web.xml注册servlet

3. 没有创建servlet对象，没有 MyServlet myservlet = new MyServlet();

4. servlet是Tomcat服务器创建的，Tomcat也称为容器。Tomcat作为容器，里面存放有servlet对象



### IoC的技术实现  

* DI(Dependency Injection) 依赖注入  

> 只需在程序中提供要使用的对象名称就行，至于对象如何在容器中创建，赋值，查找都由容器内部实现

* Spring是使用了DI实现了IoC的功能，Spring底层创建对象使用的是反射机制

 
