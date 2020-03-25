## 获取标签列表

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/tag/list</span></p>
<p>请求参数：<span style="color:#e96900">tagName：标签名，非必传</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

<p>接口说明：<span style="color:#e96900">支持标签名模糊查询。</span></p>

获取成功:
```json
{
  "code": 0,
  "message": "成功",
  "data": [
    {
      "id": 1,
      "name": "测试标签1"
    },
    {
      "id": 2,
      "name": "测试标签2"
    }
  ]
}
```