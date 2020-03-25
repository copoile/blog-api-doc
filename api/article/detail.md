## 文章详情（后台）

<p>请求方法：<span style="color:#e96900">GET</p>
<p>请求地址：<span style="color:#e96900">/article/detail/{id}</span></p>
<p>需要access_token： <span style="color:#e96900">是</span></p>
<p>需要管理员权限： <span style="color:#e96900">是</span></p>
<p>接口说明：<span style="color:#e96900">用于后台文章编辑或查看详情时调用；返回文章内容；返回分类列表，在启用分类区分子父类情况下，用于编辑时分类回显,数组顺序为[node3, node2, root]。</span></p>

获取成功：
```json
{
  "code": 0,
  "message": "成功",
  "data": {
    "id": 1,
    "original": 1,
    "categoryName": "一级分类一",
    "categoryId": 1,
    "title": "标题",
    "summary": "摘要",
    "content": "内容",
	"htmlContent": "内容",
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
    ],
    "categoryList": [
      {
        "id": 1,
        "name": "一级分类一",
        "parentId": 0
      }
    ]
  }
}
```
