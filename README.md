# my-batis
# day1
1. 搭建环境
2. 创建模块
3. 编写代码
4. 测试


# day2 
CRUD实现
1. 编写接口
2. 编写查询语句
3. 测试

# day3
配置解析：
1. 核心配置文件 mybatis-config.xml 
- transactionManager 连接数据库 数据源 dbcp c3p0 druid
- dataSource 连接池
- property 属性，比如name，password等
<br>
2. 类型别名
- `<typeAliases>`名
- 扫描包的别名是类的小写，如果非要改，则需要在实体类上加注解
<br>
3. 设置

# day4
映射器：三种方式
1. resource 类路径资源引用
2. class 绑定，接口和Mapper文件必须同名，接口和Mapper配置文件必须在同一个包下
3. name 扫描包进行绑定，接口和Mapper文件必须同名，接口和Mapper配置文件必须在同一个包下

生命周期和作用域：  
sqlSessionFactoryBuilder（创建完后即关闭）→sqlSessionFactory（连接池）→sqlSession（业务）

字段名和属性不一致方法：
1. sql字段起别名
2. resultmap 结果集映射  column是数据库中的字段，property是实体类中的属性，一一对应

日志：LOG4J，STDOUT_LOGGING

