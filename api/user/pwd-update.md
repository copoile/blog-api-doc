## 修改密码
<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/user/password/update</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">oldPassword：原密码，必传</span>
<br>
<span style="color:#e96900">newPassword：新密码，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">密码不能少于6位数。</span></p>
<p></p>
修改成功：

```json
{
  "code": 0,
  "message": "成功"
}
```