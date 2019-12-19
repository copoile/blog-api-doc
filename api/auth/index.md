## 认证

认证区分客户端，因此，登录、退出、刷新access_token接口都需要在请求头带上客户端信息。
<br>
栗子： `Authorization: Basic cGM6MTIzNDU2`
<br>
这里的`cGM6MTIzNDU2`为pc:123456经过base64加密后的密文。pc为clientId，123456为clientSecret。
