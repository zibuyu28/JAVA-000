### RPC MicroService
* RPC基础
* 分布式服务化
* Dubbo
---

#### RPC基础
* 过程
    1. 本地代理存根（stab）
    2. 本地序列化反序列化
    3. 网络通信
    4. 远程序列化反序列化
    5. 远程服务存根（Skeleton）
    6. 调用实际业务
    7. 原路返回结果
    
* 设计RPC注意点
    1. 基于共享接口还是IDL
    2. 动态代理还是AOP
    3. 序列化用文本还是二进制
    4. 基于TCP还是HTTP
    5. 服务端如何查找实现类
    6. 异常处理
    
#### 分布式服务化
* 集群：服务提供者，对等，没有分工
* 分布式：服务提供，分工协作，非复制
* ESB：所有服务都汇聚到容器，然后从容器中获取服务
* 分布式服务化：直连调用，侧边增强

#### Dubbo
* 面向接口代理高性能RPC调用
* 容错负载均衡
* 服务自动注册和发现
* 高可用扩展能力
* 运行时的流量调度
* 可视化服务治理和运维