# Spring Boot - Accessing and Adding Data

Instructor's repo: https://github.com/zachhall/SubscriberList

## Dependencies
* Spring Web
* Spring Data JPA
* H2 Database
* Spring Boot Dev Tools
* Thymeleaf

### Dependencies
Had to update my Java version in pom.xml to 1.14 to make my local JDK

### App Properties
Added a few lines to be able to access our H2 database through console and to be able to load an external SQL source

### JPA
JPA - Java Persistance API
Collection of methods and classes for storing data in a database

- Dependency: Spring Data JPA

#### Annotations
* @Entity - designates a POJO class as an entity so that we can use it with JPA
* @Id - JPA will recognize this as the object's primary key
* @GeneratedValue - allows the datbase to set the value for the field
* @Column - attribute is stored in a database column by the same name
* @CreateTimestamp - sets the value of the field to the current tima and date during creation(exactly once)

### Thymeleaf
* Thymeleaf is a server-side Java templating engine for both web and standalone JAR apps. 
* Thymeleaf sits on top of existing HTML, so we write HTML like normal and just add a few things to make it a Thymeleaf template.
* https://www.thymeleaf.org/doc/articles/standarddialect5minutes.html

#### Thymeleaf "Dialect" Basics
* ${...} : Variable expressions.
* *{...} : Selection expressions.
* #{...} : Message (i18n) expressions.
* @{...} : Link (URL) expressions.
* ~{...} : Fragment expressions.