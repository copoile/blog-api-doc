## 更新用户信息

<p>请求方法：<span style="color:#e96900">POST</span></p>
<p>请求地址：<span style="color:#e96900">/user/update</span></p>
<p>请求数据格式：<span style="color:#e96900">application/json</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p></p>

请求体json：
```json
{
  "birthday": "生日",
  "brief": "简介",
  "gender": "性别，1：男，0：女",
  "nickname": "昵称",
  "userId": "当前用户id"
}
```

<p>接口说明：<span style="color:#e96900">
生日日期格式为yyyy-mm-dd；当前用户id不可空；更新不为null的项。
</span></p>

更新成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
