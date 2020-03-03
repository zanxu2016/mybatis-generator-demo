# Mybatis逆向工程
## 步骤
### 1、创建maven项目
### 2、pom.xml文件，build->plugins->plugin，添加 mybatis-generator-maven-plugin   
> 注意此处版本问题，1.3.4及更高版本貌似有问题，还是使用`1.3.2`版本吧。
### 3、为插件添加依赖包，`mysql-connector-java`、`mybatis-generator-plugins`（此包为插件扩展包，自定义，[点击查看](https://github.com/zanxu2016/mybatis-generator-plugins)）
### 4、指定逆向工程配置文件generatorConfig.xml，具体节点含义，见配置文件中的注释
### 5、执行命令maven命令 `mvn mybatis-generator:generate`，生成entity和mappers文件