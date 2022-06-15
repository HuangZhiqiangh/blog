# blog
该博客是一个记录个人学习过程的平台


1. jwt + redis
token令牌的登录方式，访问认证速度快，session共享，安全性
redis做了令牌和用户信息的对应管理，
+ 进一步增加了安全性
+ 登录用户做了缓存
+ 灵活控制用户的过期（续期，踢掉线等）
2. threadLocal使用了保存用户信息，请求的线程之内，可以随时获取登录的用户，做了线程隔离
 
3. 在使用完ThreadLocal之后，做了value的删除，防止了内存泄漏
 
4. 线程安全-update table set value = newValue where id=1 and value=oldValue
5. 统一日志记录，统一缓存处理





