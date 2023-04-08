<<<<<<< HEAD
<<<<<<< HEAD
# miaosha
这是一个适合学完spingboot且对高并发知识有一定了解初学者学习的项目

## 实现功能
- 商品的管理
- 库存管理
- 用户管理
- 订单管理 .......
## 使用技术栈
- springboot
- mybatis
- redis
- mysql
- rocketmq......

## 下单流程(项目最重要)
1. 校验这个请求是否合法（用户是否登录、商品是否存在、活动是否开启.....）
2. redis 预扣减库存(获取操作信号量)
3. 本地事务创建订单、创建日志
4. 发送事务消息
5. 扣减存库(乐观锁更新),更新订单状态
6. 前端通过轮询的方法查看是否下单成功
> 主流程如上,但是有很多需要特别注意的地方,详细见代码注释

## 项目亮点
- 遵守分层领域模型规约
- 严格遵守alibaba java代码规范
- 项目使用的工具类均由自己封装
- 封装了限流注解
- 使用mq进行了异步操作嗯嗯嗯
  
- 使用redis guava_cache 做了多级缓存 ....

## 项目还能做哪些
### 风控相关的 
- 使用接口隐藏、验证码、请求令牌的方式 防止程序刷接口
### 系统相关
- 对页面进行静态化处理，将页面放在CDN服务器上
- LVS、nginx负载均衡横向扩展服务器
- nginx 缓存


##end
这个项目如果对你有帮助,请给我点一个免费的star吧 ，如果我项目中有错误的地方请指出 ---- email : 3117383592@qq.com


=======
# grabclass
High concurrent class rush system based on Java
>>>>>>> 489b893 (Initial commit)
=======
# grabclass
High concurrent class rush system based on Java
>>>>>>> 489b893efc50c11dd167ebf278cc5ba64d85e7bf
