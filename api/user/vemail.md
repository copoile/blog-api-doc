## 邮箱验证

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/user/email/validate</span></p>
<p>请求参数：<span style="color:#e96900">email：邮箱</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">绑定邮箱时需验证邮箱，调用成功会发送验证链接到邮箱中，链接中携带的参数code将作为绑定邮箱的凭证。
</span></p>
<p></p>
发送成功：

```json
{
  "code": 0,
  "message": "成功"
}
```