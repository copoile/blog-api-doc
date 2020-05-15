## 文章

文章分原创和转载，文章为转载时需标出文章转载地址。

### 文章数据库表设计

|字段名	    			|描述   	            		|
|:----: 				|:----:             		|
|id   					|id		            		|
|original				|是否原创，1:是，0:否	     	|
|user_id				|用户id						|
|category_id			|分类id						|
|category_name			|分类名称-冗余字段				|
|title					|文章标题						|
|summary				|文章摘要						|
|content				|文章内容						|
|hmtl_content          | 文章富文本内容              |
|status					|章状态：0为正常，1为待发布，2为回收站						|
|view_count				|文章浏览次数					|
|comment_count			|评论数-冗余字段				|
|like_count				|点赞数-冗余字段				|
|collect_count			|收藏数-冗余字段				|
|publish_time			|发布时间						|
|update_time			|更新时间						|
|reproduce				|转载地址						|
|deleted				|已删除，1：是，0否			|