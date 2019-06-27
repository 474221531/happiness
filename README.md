# -赛题背景
在社会科学领域，幸福感的研究占有重要的位置。这个涉及了哲学、心理学、社会学、经济学等多方学科的话题复杂而有趣；同时与大家生活息息相关，每个人对幸福感都有自己的衡量标准。如果能发现影响幸福感的共性，生活中是不是将多一些乐趣；如果能找到影响幸福感的政策因素，便能优化资源配置来提升国民的幸福感。目前社会科学研究注重变量的可解释性和未来政策的落地，主要采用了线性回归和逻辑回归的方法，在收入、健康、职业、社交关系、休闲方式等经济人口因素；以及政府公共服务、宏观经济环境、税负等宏观因素上有了一系列的推测和发现。

赛题尝试了幸福感预测这一经典课题，希望在现有社会科学研究外有其他维度的算法尝试，结合多学科各自优势，挖掘潜在的影响因素，发现更多可解释、可理解的相关关系。

# 赛题说明
赛题使用公开数据的问卷调查结果，选取其中多组变量，包括个体变量（性别、年龄、地域、职业、健康、婚姻与政治面貌等等）、家庭变量（父母、配偶、子女、家庭资本等等）、社会态度（公平、信用、公共服务等等），来预测其对幸福感的评价。

幸福感预测的准确性不是赛题的唯一目的，更希望选手对变量间的关系、变量群的意义有所探索与收获。

# 数据说明
complete文件为变量完整版数据，

index文件中包含每个变量对应的问卷题目，以及变量取值的含义。

survey文件是数据源的原版问卷，作为补充以方便理解问题背景。

数据来源：赛题使用的数据来自中国人民大学中国调查与数据中心主持之《中国综合社会调查（CGSS）》项目。赛题感谢此机构及其人员提供数据协助。中国综合社会调查为多阶分层抽样的截面面访调查。

外部数据：赛题以数据挖掘和分析为出发点，不限制外部数据的使用，比如宏观经济指标、政府再分配政策等公开数据，欢迎选手交流分享。

# 评测指标
提交结果为csv文件，其中包含id和happiness的预测值两列。
# 分数计算公式：
以均方误差作为判断标准

# 解决方案
其中happiness_clf是以分类形式来操作预测，但因结果是以均方误差作为判断标准，而不是以准确度作为标准，所以后续又以happiness_r提交

# 提交结果
其中happiness_clf分类错误均方误差提交为0.67，happiness_r回归错误均方误差为0.48，后续可继续用网格搜索进行模型参数优化及模型的融合
