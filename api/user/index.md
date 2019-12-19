## 用户

目前，系统用户分系统管理员和普通用户，系统管理员拥有全部权限，普通用户拥有评论、留言等权限。

### 数据库用户表设计

|字段名	    |描述   	            |
|:----: 	|:----:             |
|id   		|id		            |
|username	|用户名	     		|
|password	|密码				|
|mobile		|手机号				|
|nickname	|昵称				|
|gender		|性别，1：男 ，0：女	|
|birthday	|生日				|
|email		|邮箱				|
|brief		|个性签名			|
|avatar		|头像				|
|status		|状态，0：正常，1：锁定，2：禁用，3：过期	|
|admin		|是否管理员，1：是，0：否		|
|create_time|注册时间			|