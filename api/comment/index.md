## 文章评论与回复

支持对文章进行评论以及对文章评论进行回复。数据库表分文章评论表和文章回复表。新增评论时会发送评论提醒邮件给文章作者，新增回复时会发送回复提醒邮件给被回复者，同时抄送到文章作者。

> [!TIP]
> 发送邮件提醒需用户绑定邮箱，未绑定邮箱时最好提示未绑定邮箱，引导用户进行邮箱绑定。

### 数据库文章评论表设计

|字段名	    			|描述   	            		|
|:----: 				|:----:             		|
|id   					|id		            		|
|article_id				|文章id	     				|
|from_user_id			|评论者id					|
|content				|评论内容						|
|comment_time			|评论时间						|
|deleted				|是否删除，1：是，0：否			|

### 数据库文章回复表设计

|字段名	    			|描述   	            		|
|:----: 				|:----:             		|
|id   					|id		            		|
|article_id				|文章id	     				|
|comment_id				|评论id	     				|
|from_user_id			|回复者id					|
|to_user_id				|被回复者id					|
|content				|回复内容						|
|reply_time				|回复时间						|
|deleted				|是否删除，1：是，0：否			|