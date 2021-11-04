# tomcat-maven
## tomcat10.0.12源码maven版本
### 1. `idea` 导入
- 1.1 将代码 `git clone` 到本地 ;
- 1.2 安装好 `maven` , 配置好仓库地址 ;
- 1.3 刷新并下载依赖 `jar` 包 ;
- 1.4 将 `lib` 目录下的依赖 `jar` 包引用到依赖 .

### 2. 启动并运行 `tomcat` 源码
- 2.1. 新建 `Run/Debuge` 配置 , 增加 `jvm` 启动参数 , `catalina.home` 和 `catalina.base` 修改成下载到本地后的目录地址
```java
-Dcatalina.home=D:\dev\project\tomcat-maven\
-Dcatalina.base=D:\dev\project\tomcat-maven\
-Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager
-Djava.util.logging.config.file=conf/logging.properties
-Dfile.encoding=UTF-8
```
- 2.2 设置启动入口为 `Bootstrap` , 启动项目
```java
org.apache.catalina.startup.Bootstrap
```
- 2.3 访问 `127.0.0.1:8080` 

