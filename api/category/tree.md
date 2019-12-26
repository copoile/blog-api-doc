## 获取分类树

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/category/tree</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>

<p>接口说明：<span style="color:#e96900">获取到的数据其数据类型为树形结构。</span></p>

获取成功:
```json
{
  "code": 0,
  "message": "成功",
  "data": [
    {
      "id": 1,
      "name": "一级分类一",
      "parentId": 0,
      "children": [
        {
          "id": 3,
          "name": "二级分类一",
          "parentId": 1
        }
      ]
    },
    {
      "id": 2,
      "name": "一级分类二",
      "parentId": 0
    }
  ]
}
```