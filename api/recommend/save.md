## 保存到推荐

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/article/recommend/save</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">articleId：文章id，必传</span>
<br>
<span style="color:#e96900">score：分数，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p>接口说明：<span style="color:#e96900">只能添加已发布文章；若已添加则更新缓存；分数即为排序（顺序）。</span></p>

保存成功：
```json
{  
	"code": 0,  
	"message": "成功"
}
```
