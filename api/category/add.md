## 新增分类

<p>请求方法：<span style="color:#e96900">POST</span></p>
<p>请求地址：<span style="color:#e96900">/category/add</span></p>
<p>请求数据格式：<span style="color:#e96900">application/json</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p></p>

请求体json：
```json
{
  "name": "分类名",
  "parentId": "父id"
}
```

<p>接口说明：<span style="color:#e96900">一级分类parentId传0，若分类不需区分上下级parentId都传0即可。</span></p>

新增成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
