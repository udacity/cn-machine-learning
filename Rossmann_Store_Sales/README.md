# Forecast Rossmann Store Sales 
(from Kaggle Competition)


### 题目描述

![](./rossmann_banner2.png)

Rossmann是欧洲的一家连锁药店。 在这个源自Kaggle比赛[Rossmann Store Sales](https://www.kaggle.com/c/rossmann-store-sales)中，我们需要根据Rossmann药妆店的信息（比如促销，竞争对手，节假日）以及在过去的销售情况，来预测Rossmann未来的销售额。

### 数据下载 
此数据集可以从Kaggle上[下载](https://www.kaggle.com/c/rossmann-store-sales/data)。


### 建议

* 建模第一步就是分析你的数据集，包括特征分析、预测的目标分析等等；该任务是一个回归预测类问题，这里尤其要注意预测是未来的销量；
* 合理的划分你的训练集、验证集，记住你的目的是对于测试集的预测，这是需要提交到kaggle测评的；
* 模型层面的话，建议尝试GBDT类模型，例如xgboost、lightgbm等模型；
* 多多参考kaggle discussion，你能获得很多的优秀特征工程建议以及模型构建的技巧；


### 提交
* PDF 报告文件（注意这不应该是notebook的导出，请按照[模板](https://github.com/nd009/capstone/blob/master/capstone_report_template.md)填写）
* 项目相关代码
* 包含使用的库，机器硬件，机器操作系统，训练时间等数据的 README 文档
* 我们要求学员最低达到leaderboard private 的top 10%,对于测试集rmpse为0.11773。
[kaggle 排行榜](https://www.kaggle.com/c/rossmann-store-sales/leaderboard)



### 参考
比赛第一名的[采访](http://blog.kaggle.com/2015/12/21/rossmann-store-sales-winners-interview-1st-place-gert/)及[参考资料](https://www.kaggle.com/c/rossmann-store-sales/forums/t/18024/model-documentation-1st-place)。

[第三名的方案](https://github.com/entron/entity-embedding-rossmann)

