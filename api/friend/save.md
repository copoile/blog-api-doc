## 保存友链
<p>请求方法：<span style="color:#e96900">POST</span></p>
<p>请求地址：<span style="color:#e96900">/friend/link/save</span></p>
<p>请求数据格式：<span style="color:#e96900">application/json</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p></p>

请求体数据格式：
```json
{
  "icon": "图标",
  "id": "id",
  "name": "名称",
  "url": "链接"
}
```

<p>接口说明：<span style="color:#e96900">id为null则新增，id不为null则更新;name和url不能为空；</span></p>

保存成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
