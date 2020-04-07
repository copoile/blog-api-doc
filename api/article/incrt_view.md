## 文章浏览数自增

<p>请求方法：<span style="color:#e96900">PUT</p>
<p>请求地址：<span style="color:#e96900">/increment_view/{id}</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">20分钟内ip或用户文章浏览计数，data返回true则表示此次成功自增</span></p>

调用成功：
```json
{  
	"code": 0,  
	"message": "成功",
	"data": true
}
```
