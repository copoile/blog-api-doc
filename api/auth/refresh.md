## 刷新access_token

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/refresh_access_token</span></p>
<p>请求参数：<span style="color:#e96900">refresh_token：refresh_token，必传</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

需要[客户端认证](index.md)： <span style="color:#e96900">是</span>

<p>接口说明：<span style="color:#e96900">需要客户的启用refresh_token；access_token过期时间一般比refresh_token短，使用refresh_token刷新access_token可避免频繁登录。</span></p>

<p></p>

刷新成功：

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
