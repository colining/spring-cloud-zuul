# zuul
* zuul 主要的功能是api gateway的作用，用于于外界交流，提供路由，监控，认证等服务。
* 网关默认路由规则是使用service在Eureka上的serviceId作为对应关系的
* zuul的一大主要功能是过滤，在AccessFilter中如果没有token的话就返回401
* zuul也可以进行路由熔断，当前版本仅支持服务级别的熔断
* zuul 可以进行路由重试