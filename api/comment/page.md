## 分页获取评论与回复

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/comment/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，非必传，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，非必传，默认5</span>
<br>
<span style="color:#e96900">articleId：文章id，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

<p>接口说明：<span style="color:#e96900">评论下挂回复列表；按时间降序排序。</span></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "records": [
      {
        "id": 1,
        "content": "测试",
        "commentTime": "2020-01-05 12:52:16",
        "fromUser": {
          "id": 1,
          "nickname": "小管家",
          "avatar": "https://poile-img.nos-eastchina1.126.net/me.png",
		  "admin": 1
        },
        "replyList": [
          {
            "id": 1,
            "content": "自己回复自己可还行。",
            "replyTime": "2020-01-05 13:23:55",
            "fromUser": {
              "id": 1,
              "nickname": "小管家",
              "avatar": "https://poile-img.nos-eastchina1.126.net/me.png",
			  "admin": 1
            },
            "toUser": {
              "id": 1,
              "nickname": "小管家",
              "avatar": "https://poile-img.nos-eastchina1.126.net/me.png",
			  "admin": 1
            }
          }
        ]
      }
    ],
    "total": 1,
    "size": 5,
    "current": 1,
    "searchCount": true,
    "pages": 1
  }
}
```
