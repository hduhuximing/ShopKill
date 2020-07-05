# SpringBoot-SecondKill

#### 介绍
基于SpringBoot+Mybatis+Mysql+中间件构建的商城秒杀系统；其中，中间件主要包括：缓存中间件Redis、消息中间件RabbitMQ、统一协调调度中心中间件ZooKeeper、综合中间件Redisson等等，详细的技术列表可以参见下方“系统整体架构说明”
**(走过路过，千万要记得Fork和Star哦！！！)**

 **对应的所有博客列表** ：http://www.fightjava.com/web/index/blog/type.html?typeId=8    

 **对应的视频教程地址** ：http://www.fightjava.com/web/index/course/detail/6  

#### 系统整体架构说明
（1）技术列表：
![alt 核心技术列表](https://images.gitee.com/uploads/images/2019/0824/235302_1a4261d5_1442143.png)

（2）系统整体业务流程：
![alt 系统整体业务流程](https://images.gitee.com/uploads/images/2019/0824/235302_03ea97cd_1442143.png)

（3）系统实战收益：
![alt 系统实战收益](https://images.gitee.com/uploads/images/2019/0824/235302_0311e170_1442143.png)  

(4)部分运行效果截图：
![alt 运行效果1](https://images.gitee.com/uploads/images/2019/0824/235302_3a6851d7_1442143.png)    

![alt 运行效果2](https://images.gitee.com/uploads/images/2019/0824/235302_de1cfc85_1442143.png)   
 
![alt 运行效果3](https://images.gitee.com/uploads/images/2019/0824/235302_6cfca7e5_1442143.png)   
 

#### 开发软件与工具
IntelliJ IDEA  
DataGrid (或者 Navicat Premium)  
SpringBoot 1.5.7  
JDK1.8  
Mysql5.6  
Tomcat7 (或者 Tomcat8)  
JMeter5.x  
PostMan  
Redis_Windows的简化安装版(Redis-x64-3.2.100)--当然，如果自己有Linux服务器，也可以连接Linux的  
ZooKeeper_Windows的简化安装版(Zookeeper-3.4.6)--当然，如果自己有Linux服务器，也可以连接Linux的  
(注意：Redis_Windows的简化安装版 和 ZooKeeper_Windows的简化安装版(Zookeeper-3.4.6) 的简化版工具可以在**“附件”**中下载)

#### 如何运行整个系统  
1.首先需要在本地开发环境启动Redis、ZooKeeper服务（假设整套系统连接的服务是本地的）:双击Redis、ZooKeeper-Windows简化安装版的bin目录，Redis找寻redis-server.exe，ZooKeeper找寻zkServer.cmd文件，双击即可启动相应的服务     
2.将数据库的DDL，即db_second_kill.sql导入到你本地数据库中（前提是你得先建好数据库db_second_kill）     
3.将项目从码云check出来，并import进IDEA中，调整IDEA的maven仓库指向，最终将所需要的jar包都下载下来！(如果有一些Jar下载不下来，自己检查一下网络原因跟maven仓库原因吧!)    
4.修改application.properties配置文件中相应的配置信息，比如数据库连接信息等等；    
5.将系统运行在Tomcat服务器上，观察控制台的输出信息，如果没有报错，那么运行之后一般会自动跳转至首页！  
6.最后，可以开心的玩耍了！  

#### 博客列表(建议按照顺序来！！)  
1.Java秒杀系统(一)：Java商城秒杀系统设计与实战视频教程(SpringBoot版)重磅发布：http://www.fightjava.com/web/index/blog/article/13   
2.Java秒杀系统(二)：构建SpringBoot多模块项目：http://www.fightjava.com/web/index/blog/article/14    
3.Java秒杀系统(三)：整体业务流程介绍与数据库设计：http://www.fightjava.com/web/index/blog/article/15    
4.Java秒杀系统(四)：待秒杀商品列表与详情功能开发：http://www.fightjava.com/web/index/blog/article/16      
5.Java秒杀系统(五)：整合Shiro实现用户登录认证：http://www.fightjava.com/web/index/blog/article/17      
6.Java秒杀系统(六)：商品秒杀代码实战：http://www.fightjava.com/web/index/blog/article/18      
7.Java秒杀系统(七)：分布式唯一ID生成订单编号：http://www.fightjava.com/web/index/blog/article/19      
8.Java秒杀系统(八)：整合RabbitMQ实现消息异步发送：http://www.fightjava.com/web/index/blog/article/20        
9. Java秒杀系统(九)：开发通用的发送邮件服务：http://www.fightjava.com/web/index/blog/article/21         
10.Java秒杀系统(十)：RabbitMQ死信队列处理超时未支付的订单：http://www.fightjava.com/web/index/blog/article/22       
11.Java秒杀系统(十一)：定时任务补充处理超时未支付的订单：http://www.fightjava.com/web/index/blog/article/23       
12.Java秒杀系统(十二):JMeter压力测试重现秒杀场景中超卖等问题：http://www.fightjava.com/web/index/blog/article/24      
13.Java秒杀系统(十三)：数据库级别Sql的优化与代码的调整：http://www.fightjava.com/web/index/blog/article/25      
14.Java秒杀系统(十四)：基于Redis的原子操作优化秒杀逻辑：http://www.fightjava.com/web/index/blog/article/26    
15.Java秒杀系统(十五)：基于Redisson的分布式锁优化秒杀逻辑：http://www.fightjava.com/web/index/blog/article/27    
16.Java秒杀系统(十六)：基于ZooKeeper的分布式锁优化秒杀逻辑：http://www.fightjava.com/web/index/blog/article/28      
17.Java秒杀系统(十七)：秒杀逻辑优化之RabbitMQ接口限流一：http://www.fightjava.com/web/index/blog/article/29  
18.Java秒杀系统(十八)：秒杀逻辑优化之RabbitMQ接口限流二：http://www.fightjava.com/web/index/blog/article/30  
