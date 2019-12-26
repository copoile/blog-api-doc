## 用户状态修改

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/user/status/update</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">userId：用户id，必传</span>
<br>
<span style="color:#e96900">status：状态，必传，0:正常，1:锁定，2:禁用，3:过期</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p>接口说明：<span style="color:#e96900">用于禁用、锁定用户等操作。</span></p>
<p></p>
修改成功：

```json
{
  "code": 0,
  "message": "成功"
}
```