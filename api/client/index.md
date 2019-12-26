## 客户端

系统用户认证区分客户端，比如pc网页端、安卓客户端、ios客户端等。各客户端可自定义设置登录超时时间。

### 数据库客户端表设计

|字段名	    			|描述   	            		|
|:----: 				|:----:             		|
|id   					|id		            		|
|client_id				|客户端id	     			|
|client_secret			|客户端秘钥					|
|access_token_expire	|access_token有效时长			|
|refresh_token_expire	|refresh_token_expire有效时长|
