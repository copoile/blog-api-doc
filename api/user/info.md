## 获取用户信息

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/user/info</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">前端权限菜单可根据roleList生成；用户头像可能不存在，默认头像前端指定即可。</span></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
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
	"admin": 1,
    "roleList": [
      "admin"
    ]
  }
}
```
