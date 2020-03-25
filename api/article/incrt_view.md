## 文章浏览数自增

<p>请求方法：<span style="color:#e96900">PUT</p>
<p>请求地址：<span style="color:#e96900">/article/status/update</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">articleId：文章id，必传</span>
<br>
<span style="color:#e96900">status：文章状态，必传，值可选项，0:发布，1:待发布，2:回收站</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p>接口说明：<span style="color:#e96900">用于发布文章撤回，删除文章撤回等操作。</span></p>

修改成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
