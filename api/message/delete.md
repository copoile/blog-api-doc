## 删除留言或回复

<p>请求方法：<span style="color:#e96900">DELETE</p>
<p>请求地址：<span style="color:#e96900">/leave/message/delete/{id}</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

<p>接口说明：<span style="color:#e96900">逻辑删除；本人或管理员可删除。</span></p>

删除成功:
```json
{
  "code": 0,
  "message": "成功"
}
```