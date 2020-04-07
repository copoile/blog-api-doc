## 修改标签

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/tag/update</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">id：标签id，必传</span>
<br>
<span style="color:#e96900">name：标签名，必传</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>

<p>接口说明：<span style="color:#e96900">标签修改只可修改标签名。</span></p>

修改成功:
```json
{
  "code": 0,
  "message": "成功"
}
```