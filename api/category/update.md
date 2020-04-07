## 修改分类

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/category/update</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">id：分类id，必传</span>
<br>
<span style="color:#e96900">name：分类名，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>

<p>接口说明：<span style="color:#e96900">分类修改只可修改分类名</span></p>

修改成功:
```json
{
  "code": 0,
  "message": "成功"
}
```