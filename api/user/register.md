## 用户注册
<p>请求方法：<span style="color:#e96900">POST</span></p>
<p>请求地址：<span style="color:#e96900">/user/register</span></p>
<p>请求数据格式：<span style="color:#e96900">application/json</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p></p>

请求体json：
```json
{
  "code": "验证码",
  "mobile": "手机号",
  "password": "密码",
  "username": "用户名"
}
```

<p>接口说明：<span style="color:#e96900">验证码调发送验证码接口获取；用户名只能字母开头，允许2-16字节，允许字母数字下划线；密码不能少于6位数。</span></p>

注册成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
