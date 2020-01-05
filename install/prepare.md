
# 准备

## redis安装

项目运行依赖于redis服务，不了解redis的伙伴可以自行查阅一翻，网上的安装教程也很多，这里只放出了两个下载链接，就不做详细介绍了。
<br>
Window版下载地址: [https://github.com/microsoftarchive/redis/releases](https://github.com/microsoftarchive/redis/releases)
<br>
Linux版下载地址:[https://redis.io/download](https://redis.io/download)
<br>
这里稍微讲下redis的配置的需要注意的一个地方，默认情况下redis的访问是绑定本机访问的，如需要外网访问需要修改以下三个配置:
 ```
# 配置密码
requirepass 你的密码
# 绑定的ip
bind 0.0.0.0
# 保护模式
protected-mode no
 ```
## mysql安装

项目运行依赖于mysql服务，mysql安装篇幅稍长，网上安装教程也很多，这里放出一个安装教程链接。
[Centos7 安装 Mysql 数据库](https://cloud.tencent.com/developer/article/1329000)。
需要注意一点，字符编码最好改为utf8mb4而不是utf8，因为表情符用utf8字符编码存不下,如若确认存储的内容不含表情符也可以配置utf8。
<br>
utf8mb4字符编码配置如下:
```
character_set_server=utf8mb4
init_connect='SET NAMES utf8mb4
```
正确安装mysql好服务后，新建一个名为blog_db的数据库，字符编码集选择utf8mb4，接着初始化系统数据即可（sql文件在项目sql文件夹下）。

## 阿里云短信服务开通

项目接入阿里云短信服务，用于短信验证码发送，需要个人去[阿里云平台](https://www.aliyun.com/product/sms)开通阿里云短信服务。
短信发送需要在阿里控制台云短信模块中配置两个配置，一个是签名，所谓签名就是发送短信时前面[]的内容，
如:[阿里云]尊敬的用户：您的校验码，略。这里的<b>阿里云</b>就是签名。还有一个需要配置的就是短信模板，这个也很好理解，这个模板加上参数就是完整的短信内容。
<br>
模板栗子：
<br>
![图片](http://qiniu.poile.cn/sms.png)
> [!TIP]
> 影响短验证码接口，不影响项目启动。

## 云存储

这部分为非必须，如购买的服务器不存在带宽压力可以忽略此部分。
<br>
关于云存储，项目供[阿里云](https://www.aliyun.com/product/oss)、[网易云](https://www.163yun.com/product/nos?entry=dh01040203)、[七牛云](https://www.qiniu.com/products/kodo)三种选择。至于用哪种看个人选择，这里简单说下本人了解到的一些信息。
<br>
- 七牛云个人认证后有10G的免费存储空间，但需具备一个已备案的域名，然后新增一个记录类型为CNAME的域名解析。还有一点，默认情况下为http协议，如需https需支付额外的费用。
<br>
- 网易云之前个人认证后有50G的免费存储空间，遗憾的是目前貌似要求升级至企业级认证方可享有50G的免费存储空间。
<br>
- 阿里云40G存储空间的一个月1.00￥，买的时长越长价格越优惠。
<br>

## 系统邮箱

项目接入邮箱服务，需要配置系统邮箱，用于发送系统邮件。

> [!TIP]
> 影响部分功能，不影响项目启动。

## java环境

项目使用java语言编写，因此，需要配置java环境。java环境开发环境和生产环境都是需要配置的。网上java环境安装配置的教程很多，这里不做详细介绍，
jdk版本不低于1.8即可。

## maven环境

maven是用来下载和安装依赖、打包，类似npm的一个东西。在开发环境中，我们需要安装配置maven环境。网上maven环境安装配置的教程很多，这里也不做详细介绍，
maven版本不低于3.5即可。
> [!TIP]
> 生产环境可以不用配置maven，使用mavne将项目打包成jar后只需java环境即可运行。
