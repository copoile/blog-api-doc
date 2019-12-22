# 配置

## 须知 
项目的配置文件路径:blog-api/src/main/resources
<br>
项目配置文件为阶梯式，阶梯式写法是配置的一种简化写法,如
```
spring.test1=0
spring.test2=1
```
其阶梯式写法为:
```
spring
	test1: 0
	test2: 1
```
因此，配置文件中的配置顺序、前空格不可随意更改，有严格的要求。
<br>
## 配置文件说明
配置文件有三个:
- application.yml
- application-dev.yml
- application-prod.yml

从配置文件的名字大概就可以知道这三个配置文件的作用，application.yml为基础配置文件，application-dev.yml为开发环境配置文件，application-prod.yml为生产配置文件。
application.yml无论何种环境都会启用，而application-dev.yml和application-prod.yml只会启用其中一个，
至于启动哪个取决于application.yml中的spring.profiles.active配置。
<br>
启用开发环境栗子:
```
spring:
  profiles:
    active:
      - dev
```
如需切换生产环境将dev改为prod即可。
<br>
application.yml文件除了spring.profiles.active需要修改调整，其他地方不建议修改。

## 端口配置

```
server:
  port: 9090
```

## redis配置

配置host、port、password三项，没有密码就这样空着,其他默认即可。
```
  redis:
    host: 127.0.0.1
    port: 6379
    password: 
```

## mysql数据库配置

配置url中的ip、username、password，如果数据库端口不是3306也修改下端口，其他默认即可。

```
  datasource:
    url: jdbc:mysql://127.0.0.1:3306/blog_db?useSSL=false
    username: root
    password: root
```

## druid数据库监控配置

项目接入阿里druid数据库监控组件，可以通过web的形式查看数据库sql语句等信息。
<br>
访问路径:`http://{host}:{port}/druid/index.html`
<br>
访问的时候需要输入用户名和密码，这里的用户名和密码配置如下：
```
        login-username: admin
        login-password: password
```
用户名和密码没什么特别的要求，可自行配置。

## 系统邮箱配置

这里的邮箱配置跟Foxmail的邮箱配置差不多，没用过Foxmail的伙伴可以了解下，挺好用的一个邮件收发软件。
<br>
这里的password为授权码，没有特别说明，密码即为授权码。协议、端口等信息到对应的邮箱平台查阅。

```
  mail:
    host: smtp.163.com
    port: 25
    username: xxx@163.com
    password: password
    protocol: smtp
    default-encoding: UTF-8
    jndi-name: 个人悦读分享

```
系统邮件效果图:[http://qiniu.poile.cn/email_config.png](http://qiniu.poile.cn/email_config.png)

## 存储配置

存储配置为多选一配置，4种存储方式选择其一进行配置即可：

- 本地存储[1]
- 七牛云存储[2]
- 网易云存储[3]
- 阿里云存储[4]

生产环境配置阿里云存储栗子:
```
oss:
  type: 4
  ali:
    accessKeyId: accessKeyId
    accessKeyIdSecret: accessKeyIdSecret
    bucket: poile
    endpoint: oss-cn-shenzhen.aliyuncs.com
```
<span style="color:red">*注意*</span>:type的类型跟配置需一一对应。

## 短信验证码配置

type预留配置字段，默认1即可，expire为验证码有效时间，单位为秒，day_max为短信验证码发送接口一天内同一手机号（ip限制也是取这个值）发送验证码限制次数。
regionId固定cn-hangzhou即可。

```
sms:
  type: 1
  expire: 300
  day_max: 10
  ali:
    regionId: cn-hangzhou
    accessKeyId: 你的accessKeyId
    accessKeySecret: 你的accessKeySecret
    signName: 你的签名
    templateCode: 模板code
```

## 邮箱外链接配置

项目接入邮件服务，邮箱绑定、文章评论等会发送html邮件，点击邮箱中链接会跳转到相关页面。
邮件里的链接就是在这里配置的,至于配置什么取决于前端项目了。
```
mail:
  check: http://www.poile.cn/email/verify
  article: http://www.poile.cn/article/#/
  message: http://www.poile.cn/message
```
这里分别说下这三个链接的作用: 

1. 绑定邮箱邮箱验证链接，后面会接一个code参数，前端拿到这code后调用邮箱绑定接口进行邮箱绑定。
2. 文章评论或文章评论回复邮件提醒链接，点击跳转到文章详情页，而这里配置的就是文章详情页的前缀，后面会拼接对应的文章id
3. 留言或留言回复邮件提醒链接，点击跳转到留言页面。
