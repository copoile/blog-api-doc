## 获取用户信息

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/user/info</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">非管理员roleList为空列表</span></p>

获取成功：
```json
{
  "errorCode": 0,
  "errorMsg": "成功",
  "data": {
    "id": 1,
    "username": "admin",
    "mobile": 15625295093,
    "nickname": "小管家",
    "gender": 0,
    "birthday": "2019-07-08",
    "email": "726856005@qq.com",
    "brief": "简23介",
    "avatar": "https://poile-img.nos-eastchina1.126.net/me.png",
    "status": 0,
    "createTime": "2019-10-23T16:29:49",
    "roleList": [
      "admin"
    ]
  }
}
```