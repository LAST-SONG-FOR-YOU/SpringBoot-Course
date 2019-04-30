# SpringBoot实战系列

本项目主要基于Spring Boot框架从零开始，从最开始的项目构建、项目配置、数据存储等渐进式的进行讲解，每个章节的讲解都有之对应的源码。如果能对您有帮助，欢迎点击右上角Star按钮，给予支持！

> **作者：** 五月君，Node.js Developer，[慕课网认证作者](https://www.imooc.com/u/2667395)。
> **作者：** chy
## 宗旨

* 小项目大思想
* 以最为简洁的代码示例进行讲解
* 每一篇讲解都附带源码地址

## 项目构建

* [IntelliJ IDEA 中的Spring Initializr快速构建SpringBoot工程](/chapter1/README.md#intellig编辑器创建)
* [编写一个Hello SpringBoot程序](/chapter1/README.md#编写一个hello-springboot-程序)
     - `[运行程序]` 三种方式启动项目 [`[more]`](/chapter1/README.md#三种启动方式)
* [项目属性配置](/chapter1/README.md#项目属性配置)
    - `[项目属性配置]` application.properties文件设置配置 [`[more]`](/chapter1/README.md#后缀properties文件配置)
    - `[项目属性配置]` application.yml文件设置配置 [`[more]`](/chapter1/README.md#后缀yml文件配置)
    - `[项目属性配置]` 自定义属性配置参数间引用 [`[more]`](/chapter1/README.md#自定义属性配置及参数间引用)
    - `[项目属性配置]` 多环境动态配置 [`[more]`](/chapter1/README.md#多环境动态配置)

## 数据存储

- ### 概览
> 在介绍以下几种数据库之前少不了先说下```Spring```家族的```spring-data```，适用于关系型和非关系型数据库，简化了配置和数据库访问。例如，```Spring Data JPA```、```Spring Data MongoDB```、```Spring Data Redis```等
- ### MySql
    * [Spring-Data-Jpa简介及常用CRUD方法](/chapter2/README.md#常用方法)
    * [pom.xml增加依赖](/chapter2/README.md#添加依赖)
    * [修改配置文件 数据库Mysql、Jpa相关配置](/chapter2/README.md#mysql相关配置)
    * [Spring-Data-Jpa实现CRUD操作实例](/chapter2/README.md#实例)
    * [问题排错](/chapter2/README.md#问题排错)
- ### MongoDB
    * [MongoDB、Spring Data MongoDB简介](/chapter2/README.md#简介)
    * [pom.xml增加spring-boot-starter-data-mongodb依赖](/chapter2/README.md#添加mongodb依赖)
    * [修改配置文件 数据库MongoDB相关配置](/chapter2/README.md#修改配置文件mongodb相关配置)
    * [定义集合模型](/chapter2/README.md#定义集合模型)
    * [创建数据访问对象](/chapter2/README.md#创建继承于mongorepository的数据访问对象)
    * [创建实例实现对数据的增删改查操作](/chapter2/README.md#创建控制层实现对数据的增删改查)
- ### Redis

## AOP面向切面编程

> AOP是一种与语言无关的程序思想、编程范式。项目业务逻辑中，将通用的模块以水平切割的方式进行分离统一处理，常用于日志、权限控制、异常处理等业务中。

* [引入AOP依赖](/chapter3/README.md#引入aop依赖)
* [AOP常用注解解析](/chapter3/README.md#aop注解)
* [实现日志分割功能](/chapter3/README.md#实现日志分割功能)
    * [```@Pointcut``` 添加切入点](/chapter3/README.md#添加切入点)
    * [```@Before``` 前置通知](/chapter3/README.md#前置通知)
    * [```@After``` 后置通知](/chapter3/README.md#后置通知)
    * [```@Around``` 环绕通知](/chapter3/README.md#环绕通知)
    * [```@AfterReturning``` 返回后通知](/chapter3/README.md#返回后通知)
    * [```@AfterReturning``` 异常通知](/chapter3/README.md#异常通知)
* [一段段伪代码读懂执行顺序](/chapter3/README.md#一段段伪代码读懂执行顺序)
* [对正常、异常两种情况分别进行测试](/chapter3/README.md测试正常异常两种情况)

## 统一异常处理

* [统一返回数据结构](/chapter4/README.md#统一返回数据结构)
    * `[统一返回数据结构]` 定义接口返回数据结构
    * `[统一返回数据结构]` 数据接口字段模型定义
    * `[统一返回数据结构]` 封装接口返回方法（成功、失败）
* [统一异常处理](/chapter4/README.md#统一异常处理)
    * `[统一异常处理]` 状态消息枚举
    * `[统一异常处理]` 自定义异常类
    * `[统一异常处理]` @ControllerAdvice统一处理异常
* [测试](/chapter4/README.md#测试)
    * `[测试]` 测试正常返回及空指针系统异常
    * `[测试]` 自定义异常测试

## 单元测试

* [添加Maven依赖](/chapter5/README.md#添加maven依赖)
* [借助IntelliJ IDEA编辑器快速创建测试类](/chapter5/README.md#创建测试类)
* [Service单元测试](/chapter5/README.md#service单元测试)
* [Controller单元测试](/chapter5/README.md#controller单元测试)
* [问题汇总](/chapter5/README.md#问题汇总)

# 邮件发送

> 本篇主要介绍了Spring Boot中邮件发送，分别讲解了简单的文本邮件、HTML邮件、附件邮件、图片邮件、模板邮件。

* [添加Maven依赖](/chapter6/README.md#添加maven依赖)
* [配置文件增加邮箱相关配置](/chapter6/README.md#配置文件增加邮箱相关配置)
* [Service、Test项目代码构建](/chapter6/README.md#项目构建)
* [五种邮件发送类型讲解](/chapter6/README.md#五种邮件发送类型讲解)
    * [文本邮件](/chapter6/README.md#文本邮件)
    * [html邮件](/chapter6/README.md#html邮件)
    * [附件邮件](/chapter6/README.md#附件邮件)
    * [html内嵌图片邮件](/chapter6/README.md#html内嵌图片邮件)
    * [模板邮件](/chapter6/README.md#html内嵌图片邮件)
* [问题汇总](/chapter6/README.md#问题汇总)

#### 未完待续，持续更新中。。。