## 保存客户端
<p>请求方法：<span style="color:#e96900">POST</span></p>
<p>请求地址：<span style="color:#e96900">/client/save</span></p>
<p>请求数据格式：<span style="color:#e96900">application/json</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p></p>

请求体数据格式：
```json
{
  "accessTokenExpire": "access_Token有效时间",
  "clientId": "客户端id",
  "clientSecret": "客户端秘钥",
  "id": "id",
  "refreshTokenExpire": "refresh_token有效时间",
  "enableRefreshToken": "是否启用refresh_token,1:是，0:否"
}
```

<p>接口说明：<span style="color:#e96900">id为null则新增，id不为null则更新;超时时间单位为秒；客户端id和客户端秘钥不能为空</span></p>

保存成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
