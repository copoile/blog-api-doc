## 更换头像

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/user/avatar/update</span></p>
<p>请求数据格式：<span style="color:#e96900">multipart/form-data</span></p>
<p>请求参数：<span style="color:#e96900">file：头像文件，必传</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">文件大小不能超过5MB，文件格式只限bmp、gif、jpeg、jpeg、png、webp格式。</span></p>
<p></p>
更新成功：

```json
{
  "code": 0,
  "message": "成功"
}
```