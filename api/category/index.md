## 分类

字段parent_id用于生成树形结构的分类，分类不需要树形结构，parent_id默认都传0即可。

###数据库分类表设计

|字段名	    			|描述   	            		|
|:----: 				|:----:             		|
|id   					|id		            		|
|name					|分类名	     				|
|parent_id				|父id						|
|deleted				|是否删除，1：是，0：否			|