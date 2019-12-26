## 邮箱绑定

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/user/email/bind</span></p>
<p>请求参数：<span style="color:#e96900">code：code</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">code为邮箱验证接口发送的验证链接的参数code，前端拿到code进行邮箱绑定。
</span></p>
<p></p>
绑定成功：

```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "type": null,
    "expire": 7200,
    "access_token": "8199a799-a992-4976-84a6-86a1ccdb1af6",
    "refresh_token": "d58fdf2e-687b-4e0c-a732-ba54305b8667"
  }
}
```