## 新增点赞

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/article/like/add</span></p>
<p>请求参数：<span style="color:#e96900">articleId：文章id，必传</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

<p>接口说明：<span style="color:#e96900">不可重复点赞。</span></p>

点赞成功:
```json
{
  "code": 0,
  "message": "成功"
}
```