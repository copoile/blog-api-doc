## 分页获取分类

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/category/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，非必传，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，非必传，默认5</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>

<p>接口说明：<span style="color:#e96900">分页获取分类</span></p>

获取成功:
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "records": [
      {
        "id": 1,
        "name": "一级分类一",
        "parentId": 0
      },
      {
        "id": 2,
        "name": "一级分类二",
        "parentId": 0
      },
      {
        "id": 3,
        "name": "二级分类一",
        "parentId": 1
      }
    ],
    "total": 3,
    "size": 5,
    "current": 1,
    "searchCount": true,
    "pages": 1
  }
}
```



