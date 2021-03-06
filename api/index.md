# 接口文档

## 须知

接口响应数据格式统一为json格式，为null字段不参与json序列化，即为null的字段将不反回。
接口http请求响应状态码统一返回200，接口是否调用成功以系统返回的响应码为准。
<br>
调用需要登录的接口时需在其请求头带上access_token。
<br>
栗子：
`Authorization: Bearer 60161b7f-15dc-4acd-a011-3d821a26a92b`
<br>
## json数据格式：

```json
{  
	"code": 0,  
	"message": "成功"
}
```
<br>
```json
{  
	"code": 1001, 
	"message": "用户名或密码错误"
}
```
<br>
```json
{  
	"code": 0,  
	"message": "成功",  
	"data": 
	{    
		"access_token": "6a2dc65f-74f6-4eb6-b4d2-2eba2af4f587",
		"token_type": "Bearer",
		"refresh_token": "17456dd5-5dbd-41ec-ad4f-7cf101c9ab3e"  
	}
}
```

## 响应码

|code		|message   		    |
|:----: 	|:----:             |
|0   		|成功		        |
|1001		|用户名或密码错误		|
|1002		|用户不存在			|
|1003		|账号已禁用			|
|1004		|账号已过期			|
|1005		|账号已锁定			|
|1006		|凭证已过期			|
|1007		|不允许访问			|
|1008		|无权限访问			|
|1009		|凭证无效或已过期		|
|1010		|刷新凭证无效或已过期	|
|1011		|无效请求或请求不接受	|
|1012		|接口访问次数限制		|
|1013		|系统错误				|