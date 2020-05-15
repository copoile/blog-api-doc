## 分页获取文章（前台）

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/published/page</span></p>
<p>请求参数：
<br>
<span style="color:#e96900">current：当前页，非必传，默认1</span>
<br>
<span style="color:#e96900">size：每页数量，非必传，默认5</span>
<br>
<span style="color:#e96900">categoryId：分类id，非必传</span>
<br>
<span style="color:#e96900">tagId：标签id，非必传</span>
<br>
<span style="color:#e96900">yearMonth：年月,格式yyyy-mm，非必传</span>
<br>
<span style="color:#e96900">orderBy：排序字段，倒序，非必传，默认:publish_time;可选项：发布时间:publish_time、浏览数:view_count</span>
<br>
<span style="color:#e96900">title：标题关键字，非必传</span>

</p>
<p>需要access_token： <span style="color:#e96900">否</span></p>
<p>需要管理员权限： <span style="color:#e96900">否</span></p>
<p>接口说明：<span style="color:#e96900">只可获取到已发布的文章；可用于文章标题模糊搜索；可用于文章归档年月、分类、标签查询对应文章列表；可用于点击排行列表；可用于最新文章列表。</span></p>
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
        "status": 1,
        "viewCount": 0,
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
