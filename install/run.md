# 运行

这里介绍的是不借助IDEA等编辑器的运行方式，即打包好后再运行的一种运行方式。

## 打包

在项目根目录，即存在pom.xml文件的同级目录下执行命令：
```
mvn clean package
```
打包过程需下载依赖，时间可能较长，需耐心等待。

## 启动
打包好的文件为target文件夹下的blog-api.1.0.jar,在blog-api.1.0.jar同级目录下执行命令：
```
java -jar blog-api.1.0.jar
```
启动成功日志输出如图：

## 生产环境

生产环境项目一般需要后台运行，将打包好的jar上传到服务器后，在其同级目录下执行命令：

```
nohup java -jar blog-api-1.0.jar >root.txt 2>&1 &
```
该命令会将应用后台启动运行，并将日志输出到当前目录下root.txt文件中,命令tail -500f root.txt可监控后500行。

<br>
关闭可执行命令：
```
ps -ef|grep -v grep|grep blog-api-1.0.jar|awk '{print $2}'|xargs kill -9
```