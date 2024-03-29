# 架构原理

## 基础架构

![img](SpringCloud架构原理.png)

### 调用逻辑

> **服务注册：**当系统启动的时候会向注册中心注册自己
>
> **服务发现：**从注册中心获取可用服务地址及端口等信息
>
> **负载均衡：**当同一个服务存在多份时需要通过`Ribbon`组件进行负载均衡
>
> **服务调用：**`Feign`负责调用相应的系统
>
> **协议：**`SpringCloud`通过`http协议`