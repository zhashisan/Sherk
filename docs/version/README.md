## 0.0.3 (下版本)

- 远程服务器登录支持
- 长时间无操作后的断连/重连机制
- 默认值的支持


## 0.0.2 ( 最新 )

- FLUSH 支持
- 完善权限系统
- 增加列删除列修改列(MODIFY和CHANGE)的支持
- 修改表名的支持
- 进程池的支持 ( bug修复 )
- show processlist 的支持
- show columns 支持

## 0.0.1

- 数据库基础建设
- 多客户端的支持
- 常用命令的支持
- 配置文件的支持
- 自动化测试支持
- 权限系统的部分支持
- 等其他支持 ...

## 特性列表
> 每一版更新的时候，都会从以下特性中选出几个作为新版本的主要更新。

- LIKE模糊查找的支持

- 支持SQL : 数据库名.数据表名, COMMENT注释支持

- NULL值支持和处理

- Sharding的支持

- 数据库服务器之间的同步( 主从复制也是同理 )

- 连接查询的支持

- 内置函数的支持

- 保护操作 : 如忘记写 Where 不允许执行

- 多行SQL语句编写时的支持

- 客户端(如KeyboardInterrupt)中断处理优化

- 锁机制( 锁表和锁行 )支持

- 自动内存管理

- 事务及设置事务隔离级别

- 删除字段 alter table comments drop column reply_user_id;

- 使用多版本并发控制 ( MVCC )

- 视图的支持

- join 支持

- mysql_affected_rows() 函数支持

- insert_or_update 支持

- distinct 支持

- 用户名@主机IP 作为用户的唯一标识 ( 如 DROP Command denied to user 'root@123.123.123.123' for table 'posts' )

- truncate 截断表 和 delete from 删除表

- AUTO_INCREMENT的支持，并支持自定义设置AUTO_INCREMENT

- UNSIGNED 支持

- 返回输出的支持(不再在响应端输出)

- 主从库的升降级 (主库降级为从库, 从库升级为主库)

- PDO_Sherk 扩展，以便在 PHP 代码中实现对 Sherk 数据库的操作

- struct_field 要不要放置 在文件中的物理地址( 这样可以加快查找 )

- 所有的SQL语句都是默认自动提交的事务，redo log 和 undo log 都需要 （ 无论是否开启自动提交，都使用 transaction 日志 ）

- 部分操作是否决定都先写到日志中，而不是直接就操作，有一个系统专门负责从日志到内存到存储的操作。