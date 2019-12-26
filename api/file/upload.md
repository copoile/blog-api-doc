## 上传文件

<p>请求方法：<span style="color:#e96900">POST</p>
<p>请求地址：<span style="color:#e96900">/file/upload</span></p>
<p>请求数据格式：<span style="color:#e96900">multipart/form-data</span></p>
<p>请求参数：<span style="color:#e96900">file：文件，必传</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p>接口说明：<span style="color:#e96900">文件大小不能超过5MB，上传成功后返回文件url。</span></p>
<p></p>
上传成功：

```json
{
  "code": 0,
  "message": "成功",
  "data": "https://poile-img.nos-eastchina1.126.net/1576903866046.png"
}
```