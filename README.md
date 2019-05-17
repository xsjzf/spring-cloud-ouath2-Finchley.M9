## spring-cloud项目

### 环境：

* 开发工具：Intellij IDEA 2018.1.3
* spring-boot: **2.0.1.RELEASE**
* spring-cloud: **Finchley.M9**
* jdk：1.8
* maven:3.5.4

### 系统架构：
```
├─cloud-parent
│  │  
│  ├─cloud-auth---------------鉴权中心[9022]
│  │ 
│  ├─cloud-base---------------普通服务[9001]
│  │ 
│  ├─cloud-config-------------配置文件中心[12000]
│  │ 
│  ├─cloud-eureka-------------服务注册中心[6868]
│  │ 
│  ├─cloud-sms----------------短信服务中心[9009]
│  │ 
│  ├─cloud-common-------------公共服务模块
│  │ 
│  └─cloud-gate---------------网关
│      │ 
│      ├─cloud-gateway--------gateway网关（普通实现，仅有路由转发功能）[9011]
│      │
│      └─cloud-zuul-----------zuul网关（实现ouath2 统一鉴权）[9033]
│
```

### 功能：
* 负载均衡
* 熔断
* 消息队列
* 短信注册
* 网关
* spring security oauth2 jwt 鉴权


### 待实现：
* jwt token redis处理
* 权限数据库存储分配




