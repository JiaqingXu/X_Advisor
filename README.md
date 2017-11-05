# X_Advisor
###new sqladvisor 

#大致结构如下
### 词法解析与语法解析
* 大体采用MYSQLparse的yacc，生成解析树
###列值的选择度计算与分析
* 做成插件形式，可输入各列值选择度，也可直连数据库查询

###模拟索引与优化器
* 仿照MySQL源码mysql_select的prepare和optimize 生成各个索引的优化路径

###cost计算
* 量化优化结果。结合MySQL5.7cost相关计算（可调整参数）

争取不烂尾吧
