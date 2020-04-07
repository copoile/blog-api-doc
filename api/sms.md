## 发送验证码

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/sms/send</span></p>
<p>请求参数：<span style="color:#e96900">mobile：手机号，必传</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">默认情况下，验证码5分钟内有效，同一手机号每天只能发10次；同一ip每天只能发10次；同一手机号限流120s一次。</span></p>

> [!TIP]
> 可以手动设置验证码到redis中，类型为Strig，key为sms:code:15649xxx56，值设置你想设置的验证码。
> 接口限流基于redis实现，key前缀为limit:sms:，删除redis对应的缓存即可去掉本次限流。
<br>

发送成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
