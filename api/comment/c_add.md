## 新增评论

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/article/comment/add</span>
<p>请求参数：
<br>
<span style="color:#e96900">articleId：文章id，必传</span>
<br>
<span style="color:#e96900">content：评论内容，必传</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

<p>接口说明：<span style="color:#e96900">评论会给文章作者发送评论提醒邮件。</span></p>

评论成功:
```json
{
  "code": 0,
  "message": "成功"
}
```