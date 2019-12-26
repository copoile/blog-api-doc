## 退出

<p>请求方法：<span style="color:#e96900">DELETE</p>
<p>请求地址：<span style="color:#e96900">/logout</span></p>
<p>请求参数：<span style="color:#e96900">access_token：access_token，必传</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
需要[客户端认证](index.md)： <span style="color:#e96900">是</span>
<p>接口说明：<span style="color:#e96900">这里的access_token以请求参数形式传递而非请求头形式。</span></p>
<p></p>
退出成功：

```json
{
  "code": 0,
  "message": "成功"
}
```
