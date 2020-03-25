## 删除收藏

<p>请求方法：<span style="color:#e96900">DELETE</p>
<p>请求地址：<span style="color:#e96900">/article/increment_view/{articleId}</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">计数标识为ip或用户id；20分钟内重复调用浏览次数不会自增；data返回是否自增</span></p>

成功：
```json
{  
	"code": 0,  
	"message": "成功",
	"data": true
}
```
