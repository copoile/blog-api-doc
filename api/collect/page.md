## 分页获取收藏

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/collect/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，非必传，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，非必传，默认5</span>
</p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">查询用户收藏，并且文章处于已发布状态的文章。</span></p>
<p></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "records": [
      {
        "id": 1,
        "original": 1,
        "categoryName": "一级分类一",
        "categoryId": 1,
        "title": "标题",
        "summary": "摘要",
        "cover": "http:www.baidu.com",
        "status": 0,
        "viewCount": 2,
        "commentCount": 1,
        "likeCount": 0,
        "collectCount": 1,
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
        ]
      }
    ],
    "total": 1,
    "size": 5,
    "current": 1,
    "searchCount": true,
    "pages": 1
  }
}
```
