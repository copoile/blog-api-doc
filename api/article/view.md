## 文章详情（前台）

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/view/{id}</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">用于前台查看详情时调用；返回文章内容；返回上一篇和下一篇。</span></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "id": 2,
    "original": 1,
    "categoryName": "一级分类二",
    "categoryId": 2,
    "title": "string",
    "summary": "string",
    "content": "string",
	"htmlContent": "string",
    "cover": "string",
    "status": 0,
    "viewCount": 0,
    "commentCount": 0,
    "likeCount": 0,
    "collectCount": 0,
    "publishTime": "2020-01-02 20:24:16",
    "updateTime": "2020-01-02 20:24:16",
    "user": {
      "id": 1,
      "nickname": "小管家",
      "avatar": "https://poile-img.nos-eastchina1.126.net/me.png"
    },
    "tagList": [
      {
        "id": 1,
        "name": "测试"
      }
    ],
    "previous": {
      "id": 1,
      "title": "标题"
    },
    "next": {
      "id": 3,
      "title": "string2"
    }
  }
}
```
