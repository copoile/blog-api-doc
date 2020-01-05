## 绑定新手机号

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/user/mobile/rebind</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">mobile：新手机号，必传</span>
<br>
<span style="color:#e96900">code：验证码，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">绑定新手机号需经过验证验证原手机号步骤，且距离上一步验证时间不超过5分钟；验证码调发送验证码接口获取。</span></p>
<p></p>
绑定成功：

```json
{
  "code": 0,
  "message": "成功"
}
```