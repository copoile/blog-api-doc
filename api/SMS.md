## 发送验证码

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/sms/send</span></p>
<p>请求参数：<span style="color:#e96900">mobile</span>：手机号，必传</p>
<p>Curl栗子：curl -X POST "http://127.0.1.1:9090/sms/send?mobile=15xxxxxxxxx"</p>
<p>说明：默认情况下，验证码有效时5分钟;默认情况下，同一手机号每天只能发10次;ip限流;同一手机号限流</p>

发送成功：
```json
{  
	"errorCode": 0,  
	"errorMsg": "成功"
}
```
