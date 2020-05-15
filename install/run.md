# 运行

这里介绍的是将项目打包好后再运行的运行方式，java后端开发的伙伴使用idea打开即可。

## 打包

在项目根目录，即pom.xml文件的同级目录下执行命令：
```
mvn clean package
```
打包过程需下载依赖，耗时可能较长，需耐心等待。

## 启动
打包好的文件在target文件夹下，文件名为blog-api.1.0.jar,在blog-api.1.0.jar同级目录下执行启动命令：
```
java -jar blog-api.1.0.jar
```
启动成功日志输出如图：

## 生产环境

生产环境应用一般需在后台运行，将打包好的jar上传到服务器，在其同级目录下执行命令：

```
nohup java -jar blog-api-1.0.jar >root.txt 2>&1 &
```
该命令的作用就是让项目在后台运行并将控制台日志输出到当前目录下的root.txt文件中。使用命令tail -500f root.txt可监控后500行日志信息。

<br>
关闭可执行命令：
```
ps -ef|grep -v grep|grep blog-api-1.0.jar|awk '{print $2}'|xargs kill -9
```

> [!TIP]
> 生产环境项目启动命令和关闭命令可作为项目启动和关闭的脚本。