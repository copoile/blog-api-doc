## 获取推荐列表

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/recommend/list</span></p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">获取文章推荐列表。</span></p>
<p></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": [
    {
      "id": 1,
      "original": 1,
      "categoryName": "一级分类一",
      "categoryId": 1,
      "title": "标题",
      "summary": "摘要",
      "cover": "http:www.baidu.com",
      "status": 0,
      "viewCount": 1,
      "commentCount": 0,
      "likeCount": 0,
      "collectCount": 0,
      "publishTime": "2019-12-31 17:53:49",
      "updateTime": "2019-12-31 17:53:49",
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
      ],
      "recommendScore": 1
    },
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
      ],
      "recommendScore": 2
    }
  ]
}
```
