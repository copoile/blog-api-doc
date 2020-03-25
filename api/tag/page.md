## 分页获取标签

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/tag/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，非必传，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，非必传，默认5</span>
<br>
<span style="color:#e96900">tagName：标签名，非必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>

<p>接口说明：<span style="color:#e96900">支持标签名模糊查询。</span></p>

获取成功:
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "records": [
      {
        "id": 1,
        "name": "测试标签1"
      },
      {
        "id": 2,
        "name": "测试标签2"
      }
    ],
    "total": 2,
    "size": 5,
    "current": 1,
    "searchCount": true,
    "pages": 1
  }
}
```