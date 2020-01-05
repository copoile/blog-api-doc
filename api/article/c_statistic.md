## 分类文章统计

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/category/statistic</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">按分类计数文章数。</span></p>
<p></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": [
    {
      "id": 1,
      "name": "一级分类一",
      "parentId": 0,
      "articleCount": 1
    },
    {
      "id": 2,
      "name": "一级分类二",
      "parentId": 0,
      "articleCount": 2
    },
    {
      "id": 3,
      "name": "二级分类一",
      "parentId": 1,
      "articleCount": 0
    },
    {
      "id": 4,
      "name": "彩色",
      "parentId": 0,
      "articleCount": 0
    }
  ]
}
```
