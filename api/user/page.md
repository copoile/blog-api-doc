## 分页获取用户

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/user/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，默认5</span>
<br>
<span style="color:#e96900">username：用户名关键字，非必传</span>
<br>
<span style="color:#e96900">nickname：昵称关键字，非必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p>接口说明：<span style="color:#e96900">用于后台管理，支持用户名和昵称模糊查询。</span></p>
<p></p>
查询成功：

```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "records": [
      {
        "id": 1,
        "username": "admin",
        "mobile": 15625295093,
        "nickname": "小管家",
        "gender": 0,
        "birthday": "2019-07-08",
        "email": "15625295093@163.com",
        "brief": "简23介",
        "avatar": "https://poile-img.nos-eastchina1.126.net/me.png",
        "status": 0,
        "createTime": "2019-10-23T16:29:49",
		"admin": 1
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