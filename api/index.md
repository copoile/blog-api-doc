# 接口文档

## 须知

接口响应数据格式统一为json格式，为null字段不参与json序列化，即为null的字段将不反回。
接口http请求响应状态码统一返回200，接口是否调用成功以返回的系统错误码为准。
<br>
调用需要登录的接口时需在其请求头带上access_token。
<br>
栗子：
`Authorization: Bearer 60161b7f-15dc-4acd-a011-3d821a26a92b`
<br>
## json数据格式：

```json
{  
	"errorCode": 0,  
	"errorMsg": "成功"
}
```
<br>
```json
{  
	"errorCode": 1001, 
	"errorMsg": "用户名或密码错误"
}
```
<br>
```json
{  
	"errorCode": 0,  
	"errorMsg": "成功",  
	"data": 
	{    
		"expire": 7200,    
		"access_token": "4e9977b1-f05d-49f7-af27-615b221a6086",    
		"type": "Bearer",    
		"refresh_token": "d203dde2-52ea-43f8-b409-fd7027c77108"  
	}
}
```

## 错误码

|errorCode	|errorMsg   	    |
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
|1010		|无效请求或请求不接受	|
|1011		|接口访问次数限制		|
|1012		|系统错误			|