## 最新留言列表

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/leave/message/latest</span></p>
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
      "content": "留言测试",
      "createTime": "2020-01-05 14:17:33",
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
