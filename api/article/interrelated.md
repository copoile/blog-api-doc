## 相关文章

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/interrelated/list</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">articleId：文章id，必传</span>
<br>
<span style="color:#e96900">limit：列表数量，非必传，默认5</span>
</p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">后台实际根据分类或标签查询。</span></p>
<p></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": [
    {
      "id": 2,
      "original": 1,
      "categoryName": "一级分类二",
      "categoryId": 2,
      "title": "string",
      "summary": "string",
      "cover": "string",
      "status": 0,
      "viewCount": 1,
      "commentCount": 0,
      "likeCount": 0,
      "collectCount": 0,
      "publishTime": "2020-01-02 20:24:16",
      "updateTime": "2020-01-02 20:24:16",
      "user": {
        "id": 1,
        "nickname": "小管家",
        "avatar": "https://poile-img.nos-eastchina1.126.net/me.png"
      },
      "tagList": [
        {
          "id": 1,
          "name": "测试"
        }
      ]
    },
    {
      "id": 3,
      "original": 1,
      "categoryName": "一级分类二",
      "categoryId": 2,
      "title": "string2",
      "summary": "string2",
      "cover": "string2",
      "status": 0,
      "viewCount": 0,
      "commentCount": 0,
      "likeCount": 0,
      "collectCount": 0,
      "publishTime": "2020-01-02 20:24:36",
      "updateTime": "2020-01-02 20:24:36",
      "user": {
        "id": 1,
        "nickname": "小管家",
        "avatar": "https://poile-img.nos-eastchina1.126.net/me.png"
      },
      "tagList": [
        {
          "id": 1,
          "name": "测试"
        }
      ]
    }
  ]
}
```
