## 保存文章

<p>请求方法：<span style="color:#e96900">POST</span></p>
<p>请求地址：<span style="color:#e96900">/article/save</span></p>
<p>请求数据格式：<span style="color:#e96900">application/json</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p></p>

请求体数据格式：
```json
{
  "categoryId": "分类id",
  "content": "文章内容",
  "cover": "封面",
  "id": "文章id",
  "original": "是否原则，1:是，0:否",
  "reproduce": "转载地址",
  "summary": "文章摘要",
  "tagIds": [
    "标签id数组"
  ],
  "title": "文章标题"
}
```

<p>接口说明：<span style="color:#e96900">文章id为null时为新增，不为null时为更新；文章标签最多4个；文章为转载时，需标出转载地址；接口将文章状态置为待发布状态;保存成功返回文章id；</span></p>

保存成功：
```json
{  
	"code": 0,  
	"message": "成功",
	"data": 1
}
```
