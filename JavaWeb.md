# Web基础

![image-20250423210727662](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423210727662.png)









# 元注解

==修饰注解的注解==

![image-20250501210752034](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501210752034.png)

![image-20250501212725702](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501212725702.png)

![image-20250501212752524](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501212752524.png)

![image-20250501210810059](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501210810059.png)

![image-20250501210822255](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501210822255.png)

![image-20250501210834830](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501210834830.png)

![image-20250501210846206](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501210846206.png)

![image-20250501210915570](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501210915570.png)

![image-20250501210923828](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501210923828.png)









# 常用注解

![image-20250501164127485](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250501164127485.png)

##单元测试

```
@DisplayName设置在测试时这个测试单元的名称，否则默认为该测试方法的名称（类名首字母改成小写）
```

![image-20250419225942844](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225942844.png)

![image-20250419225946808](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225946808.png)



## SpringBootWeb

```
@RestController标识当前类为一个请求处理类（通用标识）
​		内含@ResponseBody子注解，会自动将返回的对象/集合转换成Jason格式，写入HTTP响应体
​		内含@Controller

@RequestMapping指定请求路径和请求方式(value=...,method=...)
衍生：@GetMapping 实现了RequestMapping接口，并指定请求方式为Get
	 同理还有delete，post，put
RequestMapping中有require（设置为false则可以不传入），dafaultValue（默认值）
```



## Lombok

###@Accessors

![image-20250711094818919](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250711094818919.png)

###@EqualsAndHashCode

![image-20250711095318840](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250711095318840.png)

![image-20250711095423133](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250711095423133.png)

###其他常用

![image-20250420224240123](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224240123.png)



## 控制反转

```
@Component

@Service

@Controller

@Repository
```



## 依赖注入

```
@Autowired

@Qualifier

@Resource

@Primary
```



## Mybatis(持久层)

```
@Mapper运行时自动为该接口创建一个实现类对象，并放入IOC容器中变成一个bean

@Select(...)指定要执行的SQL语句，写在接口方法上边
```

==Mapper层只要写个接口即可，不用实现方法==





## @DateTimeFormat日期格式

![image-20250523164925037](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523164925037.png)







## @Validation参数校验

==参数校验（不用if。。。else）==

==实体类也可以用==

![image-20250521210117695](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521210117695.png)

![image-20250523104006892](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523104006892.png)

![image-20250523100247219](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523100247219.png)

![image-20250523101404894](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523101404894.png)







## @JasonFormat定义转换成Jason的格式

![image-20250523113051650](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523113051650.png)











#Maven

## 介绍

![image-20250503095435283](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503095435283.png)

![image-20250419224036787](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419224036787.png)







## Maven安装

###安装

![image-20250419224428571](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419224428571.png)

![image-20250419224448903](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419224448903.png)



### 配置环境

![image-20250419224519900](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419224519900.png)





## Maven标准目录

![image-20250419224822755](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419224822755.png)





## 认识根目录pom.xml

![image-20250503100059656](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503100059656.png)





## Maven坐标（唯一标识）

==描述当前项目==

==也是定位资源的标识==

![image-20250503101602857](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503101602857.png)

![image-20250419224722380](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419224722380.png)

![image-20250419224747626](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419224747626.png)







## 模块管理（依赖继承）

==抽取公共部分，写在parent的pom.xml中==

![image-20250511212004700](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511212004700.png)

![image-20250503104847169](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503104847169.png)

![image-20250503104856885](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503104856885.png)







## 导入Maven项目

![image-20250419225047295](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225047295.png)

![image-20250419225050861](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225050861.png)

![image-20250419225055676](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225055676.png)





## 依赖

###依赖配置

![image-20250419225130581](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225130581.png)



###排除依赖

![image-20250419225142539](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225142539.png)



### 依赖传递

![image-20250503101512176](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503101512176.png)

![image-20250419225217787](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225217787.png)



### 依赖范围

![image-20250420223746065](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420223746065.png)



### 总结

![image-20250511204320400](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511204320400.png)

![image-20250419225152065](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225152065.png)







## 生命周期

###认识

==创建，使用，开发，到最后的发布==

![image-20250419225401470](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225401470.png)



###常用phase

![image-20250419225405658](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225405658.png)

![image-20250419225410889](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225410889.png)

![image-20250419225427353](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225427353.png)

![image-20250419225441149](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225441149.png)



###lifecircle、phase、goal的关系

![image-20250503102410330](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503102410330.png)

![image-20250503102628704](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503102628704.png)

![image-20250503102653681](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503102653681.png)





## Maven本质

![image-20250503103405532](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503103405532.png)





## 测试

==测试的数据要包含所有情况，尤其是边界情况==

###测试类型

![image-20250419225547506](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225547506.png)

![image-20250419225553624](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225553624.png)



### 单元测试

####JUnit

![image-20250419225626667](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225626667.png)

![image-20250419225635552](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225635552.png)

#### 断言

![image-20250419225905479](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225905479.png)

![image-20250419225914846](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225914846.png)



#### 标识

![image-20250419225942844](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225942844.png)

![image-20250419225946808](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419225946808.png)



#### Run Coverage

![image-20250419230233798](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419230233798.png)



#### 企业规范

==测试的数据要包含所有情况，尤其是边界情况==

![image-20250419230308395](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419230308395.png)





#### 常见问题解决方案

![image-20250419230957908](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419230957908.png)





## mvnw命令

![image-20250503105637498](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503105637498.png)

<img src="C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250503105647931.png" alt="image-20250503105647931" style="zoom:150%;" />











# Web

##网页请求实质

![image-20250419231350139](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419231350139.png)





## Spring

![image-20250419231905066](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419231905066.png)



###SpringBoot

![image-20250419231913100](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419231913100.png)

![image-20250419231936049](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419231936049.png)

#### SpringBootWeb

![image-20250419232311054](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419232311054.png)

![image-20250419232319682](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419232319682.png)



### Spring官方脚手架连接不上

![image-20250419232603245](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419232603245.png)

![image-20250419232629041](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419232629041.png)



### 入门程序剖析

![image-20250419232701965](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250419232701965.png)



## Http协议

==URL是完整的访问地址，URI是资源访问路径==

==完整访问路径包括http：//，资源访问路径比如/request==

![image-20250420223818129](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420223818129.png)



### 请求数据格式

![image-20250420223833408](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420223833408.png)

![image-20250420223822723](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420223822723.png)

![image-20250420223938605](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420223938605.png)

==Web服务器Tomcat会自动帮我们处理这些HttpRequest==

==服务器要的是Jason格式的时候，直接把对象或集合返回即可，服务器会自动把服务器或对象转成Jason格式==

==这个功能在@RestController中的一个子依赖中==

![image-20250420225249941](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420225249941.png)

![image-20250420225300803](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420225300803.png)

![image-20250420224006119](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224006119.png)



### 响应数据格式

==服务器要的是Jason格式的时候，直接把对象或集合返回即可，服务器会自动把集合或对象转成Jason格式==

==这个功能在@RestController中的一个子依赖中==

![image-20250420224054593](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224054593.png)

![image-20250420224041544](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224041544.png)

![image-20250420224035577](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224035577.png)

==3XX==

![image-20250420224115501](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224115501.png)

![image-20250420224131540](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224131540.png)



## SpringBootWeb案例

###常用jar包

#### ==lombok来代替getter，toString等这些冗杂的方法==

==简化实体类的定义==

![image-20250420224240123](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224240123.png)

####==hutool读取文件和String操作==

![image-20250420224247781](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224247781.png)

`字符集-UTF_8`

``不要把路径写死了``

`编译之后main和resource文件都在类目录下即classpath，则可通过类的字节码对象获取getclass（），再getClassLoader（）获取类加载器`

![image-20250420224623381](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250420224623381.png)



### 前端程序代码

![image-20250421112156786](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421112156786.png)

![image-20250421112346937](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421112346937.png)









# 分层解耦

**我们在开发过程中，要尽量让每一个接口，每一个类，每一个方法的功能尽可能单一，只管一个功能，即“单一职责原则”**

**目的：**复杂度降低，可读性更强，扩展性更好，也更利于后期的维护



## 三层架构

DAO层会面对不同的方式，比如数据库、文件、网站

除了实体类层，每个层都要有接口

![image-20250421115519304](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421115519304.png)

![image-20250421115405455](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421115405455.png)







## IOC控制反转

###常规应用

![image-20250421162232100](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421162232100.png)

###常见问题

![image-20250421163419854](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421163419854.png)

**`我们定义的bean是白色的`**

![image-20250421162248575](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421162248575.png)

![image-20250421163250733](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421163250733.png)





## DI依赖注入

###常规应用

![image-20250421171004018](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421171004018.png)

### 常见问题

![image-20250421170927321](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421170927321.png)

![image-20250421171216169](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421171216169.png)















# 数据库操作

## 认识

![image-20250422124458357](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124458357.png)





## 企业中的使用形式

![image-20250421173820669](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250421173820669.png)





## 之前不熟悉的SQL

### DDL创建

####数据库

![image-20250422124535403](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124535403.png)

![image-20250422124542728](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124542728.png)

**![image-20250422124549110](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124549110.png)**

#### 表

![image-20250422124619363](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124619363.png)

![image-20250422124819828](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124819828.png)

#### 注意事项

==注意创建表时根据需求运用合适的数据类类型，不要浪费空间，而且注意是否能支持负数、是否唯一、是否能为空等限制==

![image-20250422124653397](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124653397.png)

#### 设计表的思路

![image-20250422124810749](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124810749.png)





### DML增删改查

![image-20250422124908990](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124908990.png)

![image-20250422124912040](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124912040.png)

==delete没有where条件时跟drop一样会删表==

![image-20250422124915744](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124915744.png)





### DQL查询

![image-20250422124938499](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124938499.png)

![image-20250422124947418](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422124947418.png)

==distinct可以去重==

![image-20250422125001900](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125001900.png)

#### 条件查询

![image-20250422125030153](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125030153.png)

![image-20250422125033173](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125033173.png)

![image-20250422125038828](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125038828.png)



#### 分组查询

![image-20250422125107503](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125107503.png)

![image-20250422125118435](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125118435.png)

![image-20250422125121488](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125121488.png)

![image-20250422125128131](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125128131.png)



#### 排序查询

![image-20250422125157389](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125157389.png)

![image-20250422125200892](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125200892.png)

![image-20250422125213727](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125213727.png)



#### 分页查询

==MySQL的行数索引是从0开始的，即第0行==

![image-20250422125223412](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422125223412.png)







## 数据库连接

### JDBC

==**JDBC是Java中操作数据库的底层基础技术**==

**==不用自己导入jar包==**

![image-20250422091504121](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422091504121.png)







### 相比的好处

==**改Java代码需要重新编译，而在配置文件中就不用**==

==配置时需要改一下字符编码格式，改成UTF-8==

![image-20250422225232768](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422225232768.png)





###==Mybatis==

#### 认识

![image-20250422142254912](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422142254912.png)



#### 使用

![image-20250422142813210](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422142813210.png)



![image-20250422144345096](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422144345096.png)

![image-20250422144738283](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422144738283.png)



#### 辅助配置

**SQL语句辅助提示，日志输出**

##### SQL提示

![image-20250422223144212](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422223144212.png)

![image-20250422223901808](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422223901808.png)

##### 日志

![image-20250422225359230](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422225359230.png)

![image-20250422225330307](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250422225330307.png)



#### 数据库连接池

##### 优点

![image-20250423095359467](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423095359467.png)

##### 认识

![image-20250423094443161](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423094443161.png)

##### 指定连接池

![image-20250423094658024](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423094658024.png)



#### 增删改查

##### 占位符

![image-20250423101146095](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423101146095.png)

##### 删除操作

![image-20250423100704215](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423100704215.png)

##### 插入增加

==注意：多个属性时最好用类封装==

==private属性也一样==

![image-20250423101849343](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423101849343.png)

##### 查询

###### 规范

==2个及2个以上的形参才要加注解==

==加了注解那么会根据注解中的名字来对应==

![image-20250423174359280](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423174359280.png)

######官方骨架的区别

![image-20250423173809217](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423173809217.png)

![image-20250423173932101](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423173932101.png)

![image-20250423174157595](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423174157595.png)



#### 映射配置文件

==配置文件放在resources中==

==全类名也叫全限定名，包名+类名==

##### 认识

![image-20250423180313733](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423180313733.png)

#####映射xml文件定义规则

![image-20250423175726321](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423175726321.png)

##### 使用情况

==一般会结合实际情况，两者结合使用==

![image-20250423180555053](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423180555053.png)

##### 辅助配置

![image-20250423202839528](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423202839528.png)









#----------------------------

#Web进阶











# 常识

```
看报错信息时要从下网上看：
从Cause by开始看，找“Cause By”关键字
SQL语句异常要找“near”
```

```
Java目录和resource目录都在同个class字节码文件中（都在main里）
模块：module
一个项目中可以有多个模块
```

```
Object.equals(A,B)
Object.hashcode(A,B)防止A,B中有null
比较器comparetor必须有-1，0，1三种返回值
```

```
做项目基本是用工具类来实现，底层的原始代码比较少



不变的量将其变为静态常量
常变的量一般以参数的形式传进来
```













# 特性

## 起步依赖

![image-20250520215618673](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250520215618673.png)













## 自动配置

==在yml配置文件配置相关信息后，会自动读取，然后注入到IOC容器中==

![image-20250520215606859](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250520215606859.png)





### 原理

![image-20250521163725610](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521163725610.png)

![image-20250521163810201](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521163810201.png)

![image-20250521164101265](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521164101265.png)











## 其他特性

![image-20250520215546119](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250520215546119.png)





















# 项目创建

![image-20250520220740433](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250520220740433.png)

![image-20250520221301085](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250520221301085.png)













# SpringBoot项目配置文件

==大部分情况下我们所写的配置只管写，不用读，我们定义对象时用@Autowired会自动读取==

==除非是我们自己写的，那么就要从配置文件中读取==

## properties文件的问题

![image-20250423203231851](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423203231851.png)



## ==yml配置文件==

==**开发常用**==

![image-20250423205542311](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423205542311.png)

![image-20250423210302581](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423210302581.png)









# 开发规范

## 开发前

==开发之前要先明确实现这个功能三层架构分别要干什么==

==准备工作：创建需要的对应表，实体类，三层架构，sql语句==

==这块功能该怎么实现？要用什么技术？请求参数该怎么接收？SQL语句该怎么编写？三层架构分别实现什么？==

==动手能力，分析问题，解决问题的能力，并学会用ai提示提效率（一定要检查ai写的代码）==

==mapper层的方法名不要用service层的名==

![image-20250429100616283](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250429100616283.png)







## 开发模式

==前后端分离，基于API文档开发==

**==接口文档，“接口”指的是功能==**

**==是基于页面和需求文档总结分析出来的==**

![image-20250423213942126](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423213942126.png)

![image-20250423214134813](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423214134813.png)

![image-20250521171953149](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521171953149.png)









## 软件架构风格

![image-20250423215303114](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423215303114.png)

![image-20250423215620488](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423215620488.png)



## 现有问题

![image-20250423220036935](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423220036935.png)



## Apifox

![image-20250423220218255](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423220218255.png)

![image-20250423221030047](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250423221030047.png)







## Result类返回类型

==Result类，统一返回格式==

![image-20250521204608113](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521204608113.png)











# 项目案例

## 部门、员工管理（接收前端数据）

### 表结构设计

==一张表除了业务字段，还要有基础字段，包括主键id，create_time，update_time==

==子表的create_time，update_time是跟着主表走的（即一致）==

![image-20250509105138750](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250509105138750.png)









### 请求头获取（Query参数）

####方式一

![image-20250508162337886](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508162337886.png)

![image-20250508161857771](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508161857771.png)



#### 方式二

#####单个值

==也可以直接用对象作为形参，会直接根据相同名字的属性名去赋值==

==mybatis中的占位符位置的变量也会自动与该类的属性名自动匹配==

![image-20250508162507886](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508162507886.png)



##### 多个值

![image-20250512204356429](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512204356429.png)





#### 总结

![image-20250508163903537](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508163903537.png)









### 请求体获取（Jason格式）

==也可以一个一个同名变量来接收==

![image-20250508165054558](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508165054558.png)

![image-20250508170703528](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508170703528.png)









### 请求头获取url路径参数

![image-20250508203042819](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508203042819.png)

![image-20250508203743981](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508203743981.png)



![image-20250508203939575](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508203939575.png)









### 参数校验

#### @Validation参数校验

==参数校验（不用if。。。else）==

==实体类也可以用==

![image-20250521210117695](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521210117695.png)

![image-20250523104006892](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523104006892.png)

![image-20250523100247219](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523100247219.png)

![image-20250523101404894](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523101404894.png)





#### 分组校验

![image-20250523121033809](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523121033809.png)

![image-20250523121353690](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523121353690.png)

![image-20250523120647150](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523120647150.png)





#### 自定义校验

==解决一个属性不同请求下的校验标准不同==

![image-20250523151753652](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523151753652.png)

==自定义注解==

![image-20250523151645753](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523151645753.png)

==自定义校验规则==

![image-20250523151439042](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523151439042.png)

![image-20250523151507548](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523151507548.png)







###Mapper层用类对占位符赋值

![image-20250508205755048](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508205755048.png)









### 日志技术

#### 介绍

![image-20250508212740246](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508212740246.png)

#### LockBack

![image-20250508213857115](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508213857115.png)

![image-20250508214024714](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508214024714.png)



#### 日志级别

![image-20250508221758904](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508221758904.png)

![image-20250508222731303](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508222731303.png)

![image-20250508222845950](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508222845950.png)









### 多表问题处理

![image-20250509094726808](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250509094726808.png)

![image-20250509100431415](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250509100431415.png)

![image-20250509101802104](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250509101802104.png)









### 多表查询

==看哪些数据需要完整来选择连接方式==

![image-20250509110014054](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250509110014054.png)









### 分页查询

#### 原始方式

![image-20250509155132539](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250509155132539.png)





#### ==PageHelper插件==

==Lombok已经依赖传递下来了==

==PageHelper中有Page类，所以那里有强转==

![image-20250523163917295](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523163917295.png)

![image-20250509163330011](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250509163330011.png)

![image-20250510211036849](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510211036849.png)

![image-20250523164322403](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523164322403.png)



![image-20250510210931101](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510210931101.png)

![image-20250510210807004](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510210807004.png)









### ==代码优化==

#### 1.请求地址在类上定义

![image-20250508210143033](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508210143033.png)

![image-20250508210531703](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250508210531703.png)





#### 2.接收前端参数

![image-20250510221722080](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510221722080.png)





#### ==3.动态SQL语句==

==例如对于条件不确定有多少项，这种时候就要用到动态SQL，根据实际情况自动调整==

#####where条件判断（多个）

![image-20250510223553474](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510223553474.png)

![image-20250510223732847](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510223732847.png)





##### values批量插入

![image-20250511101525810](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511101525810.png)

![image-20250511101438577](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511101438577.png)





##### update要更新的字段不固定

![image-20250512224148915](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512224148915.png)





##### if语句

![image-20250513104553313](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513104553313.png)

![image-20250513105312874](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513105312874.png)





##### case...when...

![image-20250513092753547](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513092753547.png)





##### concatSQL语句

==拼接作用==

![image-20250523170211252](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523170211252.png)







#### ==4.主键回显==

![image-20250511101350370](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511101350370.png)



####5.模糊匹配（concat拼接）

![image-20250510220249037](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510220249037.png)

![image-20250510215718293](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510215718293.png)

![image-20250510220000774](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250510220000774.png)





#### 6.复杂的SQL语句

==mybatis中mapper层的sql语句可以通过注解和同包同名的映射配置文件来定义==

![image-20250523170914122](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523170914122.png)





#### ==7.手动设置数据封装方式==

==笛卡尔积时如何封装数据到对象中，比如这个对象中有List，一个员工匹配多段工作经历==

![image-20250512215232748](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512215232748.png)

![image-20250512214815110](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512214815110.png)





####8.参数配置化

常见：mybatis，日志级别，阿里云OSS

便于项目的维护和统一管理

![image-20250512171746015](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512171746015.png)

![image-20250512173448653](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512173448653.png)



![image-20250512173429224](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512173429224.png)





#### 9.驼峰式命名与下划线名字自适应

==将驼峰式命名和SQL语句命名格式自动对应==

![image-20250521225754674](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521225754674.png)

![image-20250521225937079](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521225937079.png)











### 事务管理

#### 控制事务

==在service层开启和结束事务==

![image-20250511110823177](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511110823177.png)



#### rollbackfor（异常时回滚）

![image-20250511111801036](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511111801036.png)



#### propagation（事务传播）

![image-20250511115420751](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511115420751.png)

![image-20250511115017171](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511115017171.png)



![image-20250511115115600](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511115115600.png)



#### 事务四大特性

![image-20250511115300764](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250511115300764.png)









### ==文件上传==

#### 简介

![image-20250512100237791](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512100237791.png)



#### 当地存储

![image-20250512100202738](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512100202738.png)

![image-20250512102615349](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512102615349.png)





#### 第三方服务器存储

![image-20250524100949954](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250524100949954.png)

![image-20250512105447572](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512105447572.png)



![image-20250512111711368](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512111711368.png)

==拿到Accesskey之后在cmd中以管理员身份运行，配置到系统==

![image-20250512163710547](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512163710547.png)

![image-20250512162501142](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512162501142.png)

![image-20250512170951261](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512170951261.png)

![image-20250512170849094](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512170849094.png)







### ==全局异常处理器==

#### 优点



![image-20250512230817311](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512230817311.png)

![image-20250512231003534](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512231003534.png)



#### 代码示例



![image-20250512231415824](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512231415824.png)



#### 原理与总结

![image-20250512231305650](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512231305650.png)

![image-20250512230726980](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250512230726980.png)















##登录验证

### ==会话技术==

#### 介绍

![image-20250513182756850](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513182756850.png)

![image-20250513184645016](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513184645016.png)





#### Cookie技术

![image-20250513190938691](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513190938691.png)

![image-20250513190701317](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513190701317.png)

![image-20250513190903021](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513190903021.png)





#### Session技术

![image-20250513200429676](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513200429676.png)

![image-20250513200604868](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513200604868.png)





#### ==令牌技术（主流）==

==JWT身份校验==

==这些代码不用记，知道原理即可，开发时一般都是提供了工具类来使用==

##### 优点

![image-20250513201123077](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513201123077.png)



##### 介绍

==在base64编码中是补位符号==

![image-20250521220345031](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521220345031.png)



##### 实现

==作为工具类（不要加@Test）==

![image-20250521220704783](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521220704783.png)

![image-20250514153302850](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514153302850.png)



##### 总结

![image-20250513221024916](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513221024916.png)











### 过滤器Filter

#### 介绍

![image-20250513230452663](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513230452663.png)





#### 令牌校验Filter-代码示例

![image-20250513230430774](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513230430774.png)

![image-20250514095759981](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514095759981.png)

==令牌解析如果不符合会抛出异常，所以要try...catch...==

![image-20250514095835034](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514095835034.png)

![image-20250514095901821](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514095901821.png)







#### 执行流程

![image-20250514100604052](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514100604052.png)





#### 拦截路径

![image-20250514101047102](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514101047102.png)





#### 过滤器链

![image-20250514101900924](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514101900924.png)





####总结

![image-20250513230350039](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250513230350039.png)













### ==拦截器Interceptor==

#### 介绍

![image-20250514111211164](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514111211164.png)





#### 代码示例

![image-20250514111143122](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514111143122.png)

![image-20250521224613697](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521224613697.png)

==最好加上addPathPattern指定要拦截的所有路径，一般是/**==

![image-20250521224718200](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521224718200.png)

![image-20250521224449793](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521224449793.png)







#### 拦截路径

![image-20250515090059569](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515090059569.png)





#### 执行流程（与Filter的区别）

![image-20250515090837994](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515090837994.png)





#### 总结

![image-20250514111118502](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250514111118502.png)





















## ==SpringAOP==

###认识

![image-20250519093034490](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519093034490.png)





### 优点

![image-20250515091954037](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515091954037.png)





### 代码示例

![image-20250515094432073](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515094432073.png)





### 核心概念

![image-20250515095540298](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515095540298.png)



#### 连接点

![image-20250515151441163](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515151441163.png)





#### 通知

#####类型

![image-20250515105115680](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515105115680.png)



##### 顺序

![image-20250515110617752](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515110617752.png)







#### 切入点表达式

##### execution

![image-20250515113457842](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515113457842.png)



![image-20250515114036379](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515114036379.png)



![image-20250515113727140](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515113727140.png)

==execution是主流的方式，但多个逻辑运算符时不太合适==



#####@annotation

==@annotation括号内是该注解的全类名==

==添加了这个自定义注解的类/方法则会进行这个AOP程序==

![image-20250515150013824](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515150013824.png)

![image-20250515145636290](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515145636290.png)





##### @PointCut抽取切入点表达式

![image-20250515105504632](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515105504632.png)









### 执行流程（原理）

![image-20250515100357782](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515100357782.png)

==AOP的底层是动态代理技术==

==所以实际调用的是代理的方法，不再是直接调用目标方法==

![image-20250515100549080](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515100549080.png)

==连接点是可以被AOP控制的，但有些我并不想控制而已==

==切入点表达式，那些方法可以被调用，这些就是切入点==

==通知方法==





### 总结

![image-20250515094358437](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515094358437.png)











## ThreadLocal

==ThreadLocal可以存放任意类型的数据，包括lambda表达式==

![image-20250515210837725](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515210837725.png)

![image-20250515164944281](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515164944281.png)

![image-20250523094612023](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523094612023.png)

![image-20250523094507982](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250523094507982.png)















# 原理篇

## 配置优先级

==以端口号port为例==

![image-20250515214358589](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515214358589.png)

![image-20250515214339103](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250515214339103.png)









## Bean管理（面试常考）

### Bean扫描

![image-20250521092538110](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521092538110.png)













### Bean注册

####@Bean与@Import

![image-20250521094110205](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521094110205.png)

![image-20250521100642884](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521100642884.png)

==文件中存的一般是要导入的配置类的全面类名==

==ImportSelector实现类一般是总的导入类==

![image-20250521100859814](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521100859814.png)

![image-20250521100315417](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521100315417.png)









###作用域（单例与多例）

![image-20250516091932084](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250516091932084.png)



![image-20250516092210664](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250516092210664.png)





### 第三方Bean（@Bean）

==同属于springIOC容器内才能互相使用@Autowired==

![image-20250516094100223](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250516094100223.png)



![image-20250516094145870](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250516094145870.png)











## SpringBoot原理

### 起步依赖

![image-20250516094918936](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250516094918936.png)







### 自动配置

#### 实现方案

![image-20250516103609751](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250516103609751.png)

![image-20250516105954883](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250516105954883.png)





#### 源码

![image-20250517100933475](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517100933475.png)

![image-20250517100732616](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517100732616.png)







#### @Conditional

![image-20250517102828369](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517102828369.png)

![image-20250521104554996](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521104554996.png)

![image-20250521104650231](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250521104650231.png)











#### 总结

![image-20250517102812307](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517102812307.png)









### 自定义starter

#### 介绍

![image-20250517111306892](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517111306892.png)





#### 实现

![image-20250517114713766](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517114713766.png)

==规范：==

==autoconfiguration中尽量减少不必需的依赖==

==starter中只保留了pom文件，无Java代码，pom文件中导入autoconfiguration==

==autoconfiguration定义类和方法，以及其他依赖==

==其他模块导入starter依赖即可==

==在autoconfig自动配置类中导入的依赖要在starter中同步导入，方便后续的exclusive排他==

###### 实体类

![image-20250517120006893](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517120006893.png)



###### 功能类

![image-20250517120114104](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517120114104.png)



###### 配置类

![image-20250517115658959](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517115658959.png)



###### 自动配置文件

==学那些starter照猫画虎==

![image-20250517115729229](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517115729229.png)



![image-20250517115913488](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250517115913488.png)















# Maven高级

## 分模块设计

### 优点

![image-20250518103329106](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518103329106.png)





### 方式

![image-20250518105633973](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518105633973.png)





### 总结

![image-20250518105548304](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518105548304.png)













## 继承

### 实现与优点

==把各个工厂共有的依赖配置在父工程中==

![image-20250518111752941](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518111752941.png)

==一般项目中有这两种形式==

![image-20250518115033708](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518115033708.png)

![image-20250518115000718](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518115000718.png)







### 版本锁定

![image-20250518222034269](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518222034269.png)





### 代码优化<properties>

![image-20250518222016482](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518222016482.png)



![image-20250518221830053](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518221830053.png)















## 聚合

==一块打包等生命周期lifecycle操作==

![image-20250518223818093](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518223818093.png)



![image-20250518223743513](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518223743513.png)













## 私服

==解决团队内部的资源共享和资源同步的问题==

![image-20250518224539644](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518224539644.png)

![image-20250519102414642](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519102414642.png)





### 实现（应用）

![image-20250519102338176](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519102338176.png)





![image-20250519102459902](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519102459902.png)

![image-20250519102516719](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519102516719.png)

![image-20250519102530219](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519102530219.png)

![image-20250519102541786](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519102541786.png)

![image-20250519102557634](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250519102557634.png)













# ----------------------------

#总结

![image-20250518232701129](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518232701129.png)



![image-20250518233000671](C:\Users\lwh\AppData\Roaming\Typora\typora-user-images\image-20250518233000671.png)

