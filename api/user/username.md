## 绑定用户名

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/user/username/bind</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">username：用户名，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">该接口只用于原用户名为空时（第三方登录）绑定用户名。</span></p>
<p></p>
绑定成功：

```json
{
  "code": 0,
  "message": "成功"
}
```