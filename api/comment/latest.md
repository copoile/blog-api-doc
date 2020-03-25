## 最新评论列表

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/comment/latest</span></p>
<p>请求参数：<span style="color:#e96900">limit：数量，非必传，默认5</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": [
    {
      "id": 1,
      "content": "测试",
      "commentTime": "2020-01-05 12:52:16",
      "article": {
        "id": 1,
        "title": "标题"
      },
      "fromUser": {
        "id": 1,
        "nickname": "小管家",
        "avatar": "https://poile-img.nos-eastchina1.126.net/me.png",
		"admin": 1
      },
      "replyList": []
    }
  ]
}
```
