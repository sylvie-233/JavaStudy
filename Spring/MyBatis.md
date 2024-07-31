# MyBatis


## 基础介绍

### mybatis-config.xml

mybatis核心配置文件

```xml
<configuration>
    <environments> // 配置环境
        <environment>
            <transactionManager /> // 1.数据库事务管理器
            <dataSource /> // 2.数据库连接信息
        </environment>
    </environments>

    <mappers> // 3.配置数据库映射文件
        <mapper />
        <package /> // 包扫描
    </mappers>

    <typeAliases>
        <package /> // 定义类型别名（resultType简化）
    </typeAliases>
</configuration>
```

### mapper.xml

mapper操作定义文件

```xml
<mapper
    namespace= 命名空间（通常为包路径）
>
    <resultMap /> // 字段映射
    <select // 查询语句
        id= 方法名
        resultType= 返回值类型
    >

    </select>
    <insert />
    <update />
    <delete />


</mapper>
```

## 核心内容


### SqlSession

MyBatis操作的核心对象，可以使用`mapper`中定义的操作

自动事务提交




### Mapper代理

每个mapper.xml映射到一个具体的接口/类上

SQL映射文件中的namespace应该为Mapper的全限定包路径

一个代理类对应一个文件，使用SqlSession获取代理类

数据添加主键id返回


### 动态SQL

sql片段：`<sql>`，引入sql片段`<include>`

数据库字段映射：`<resultMap>`

条件查询：`<where>`、`<if>`、`<choose>/<when>/<otherwise>`

修改：`<set>`

循环：`<foreach>`


### 注解开发

`@Select`

`@Update`

`@Delete`

`@Insert`