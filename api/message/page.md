## 分页获取留言与回复

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/leave/message/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，非必传，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，非必传，默认5</span>
</p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

<p>接口说明：<span style="color:#e96900">留言下挂回复列表；按时间降序排序。</span></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "records": [
      {
        "id": 1,
        "content": "留言测试",
        "createTime": "2020-01-05 14:17:33",
        "fromUser": {
          "id": 1,
          "nickname": "小管家",
          "avatar": "https://poile-img.nos-eastchina1.126.net/me.png",
		  "admin": 1
        },
        "replyList": [
          {
            "id": 2,
            "content": "留言回复",
            "createTime": "2020-01-05 14:35:53",
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
