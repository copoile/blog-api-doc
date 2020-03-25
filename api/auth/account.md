## 账号密码登录

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/account/login</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">username：用户名/手机号，必传</span>
<br>
<span style="color:#e96900">password：密码，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
需要[客户端认证](index.md)： <span style="color:#e96900">是</span>
<p>接口说明：<span style="color:#e96900">账号可以是用户名，也可以是手机号。</span></p>
<p></p>
登录成功：

```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "access_token": "6a2dc65f-74f6-4eb6-b4d2-2eba2af4f587",
    "token_type": "Bearer",
    "refresh_token": "17456dd5-5dbd-41ec-ad4f-7cf101c9ab3e"
  }
}
```
