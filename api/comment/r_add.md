## 新增评论回复

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/article/reply/add</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">articleId：文章id，必传</span>
<br>
<span style="color:#e96900">commentId：评论id，必传</span>
<br>
<span style="color:#e96900">toUserId：被回复者id，必传</span>
<br>
<span style="color:#e96900">content：回复内容，必传</span>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>

<p>接口说明：<span style="color:#e96900">评论回复会发送回复提醒邮件给被回复者，同时也会超送到文章作者。</span></p>

回复成功:
```json
{
  "code": 0,
  "message": "成功"
}
```