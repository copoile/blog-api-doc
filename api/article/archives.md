## 文章归档

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/archives/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，非必传，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，非必传，默认12</span>
</p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">按年月归档，月份文章计数。</span></p>
<p></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "records": [
      {
        "yearMonth": "2020-01",
        "articleCount": 2
      },
      {
        "yearMonth": "2019-12",
        "articleCount": 1
      }
    ],
    "total": 2,
    "size": 12,
    "current": 1,
    "searchCount": true,
    "pages": 1
  }
}
```
