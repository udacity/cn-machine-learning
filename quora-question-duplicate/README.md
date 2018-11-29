## Quora句子相似度匹配

### 准备工作


优达学城推荐学生安装 [Anaconda](https://www.continuum.io/downloads)，这是一个常用的Python集成编译环境，且已包含了本项目中所需的全部函数库。我们在P0项目中也有讲解[如何搭建学习环境](https://github.com/nd009/titanic_survival_exploration/blob/master/README.md)。

### 题目描述

[Quora Querstion Pairs数据集](https://data.quora.com/First-Quora-Dataset-Release-Question-Pairs)是Quora于2017年公开的句子匹配数据集，其通过**给定两个句子的一致性标签标注，从而来判断句子是否一致。**

Quora 数据集训练集共包含40K的句子对，且其完全来自于Quora网站自身，Quora在发布数据集的同时，在Kaggle平台，发起了[Quora句子相似度匹配大赛](https://www.kaggle.com/c/quora-question-pairs)，共有3307支队伍参加了本次句子相似度匹配大赛，参赛队伍不仅包括来自麻省理工学院、伦敦大学学院、北京大学、清华大学、中科院计算所等高校研究所，也包括了来自微软、Airbnb、IBM等工业界的人员。

我们这里要求你使用Kaggle端的数据集，其由Train,Test两部分构成，你需要通过在Train数据集上进行验证集划分、建模，在Test数据集上进行测试，并且提交到Kaggle进行测评。

**【IMPORTANT】**数据集下载地址：[Quora DataSet](https://www.kaggle.com/c/quora-question-pairs),请注册kaggle之后，点击同意加入比赛，方可下载数据集。

数据集描述：


|  | Train | Test | 
| ------ | :-----: | :----: |
| Data Size | 404290 | 2345796 |
| Vocab Size | 95603 | 101049 |


### 题目特点

句子相似度匹配涉及了海量的自然语言处理领域的基本任务，其是检索任务、对话任务、分类任务的基础。通过该赛题你可以**有选择的**学习到自然语言处理领域方方面面的知识，并且能为你在自然语言处理相关的实际工作中提供思路。


### 预备知识

* NLP基础，包括词袋模型、TF-IDF算法、主题模型（PCA、LDA、NMF)
* 相关模型，包括Logistic Regression,GBDT(Xgboost,lightgbm),RandomForest
* 句子相似度测度， 包括余弦相似度、编辑距离、Word Mover Distance
* 这里学员可以根据自己的基础，选择是否使用深度学习类模型，深度类模型对于该题并不是必须的

部分参考链接：
1. 特征工程：
   * 一个非常完善的特征工程思路： https://www.linkedin.com/pulse/duplicate-quora-question-abhishek-thakur/

   * 特征工程部分的参考代码： https://github.com/abhishekkrthakur/is_that_a_duplicate_quora_question

   * 该比赛的一个解决方案： https://github.com/qqgeogor/kaggle-quora-solution-8th

2. 深度类模型(可选）
   * ARC I https://arxiv.org/abs/1503.03244
   * Siamese-CNN https://arxiv.org/pdf/1702.03814.pdf
   * Siamese-LSTM https://arxiv.org/pdf/1702.03814.pdf
   * Multi-Perspective-CNN https://arxiv.org/pdf/1702.03814.pdf
   
   
### 建议

在撰写报告的时候，可以侧重于理论知识方面的论述，例如关于NLP的一些基本知识（词袋模型，主题模型，TF-IDF等），以及非常常用的模型算法，例如Logistic Regression, GBDT(Xgboost,lightgbm), RandomForest；以及基本的相似度度量方法等。在你的报告你可以加上深度类模型，即使你在试验部分没有进行建模，这也将有助于你了解学习最新的相关知识。

在进行算法试验的过程中，注意对于你的特征工程有较好的记录，例如整理成表格形式；另外也建议不同类型的特征工程的生成代码可以独立开，这样更加方便你的调试。

模型融合部分，可以尝试最简单的加权平均方法，也可以直接使用更加复杂的Stacking[这里是一个较好的STACKING代码框架](https://github.com/qqgeogor/kaggle-quora-solution-8th),相关模型融合资料可以参考[这里](https://mlwave.com/kaggle-ensembling-guide/)

### 要求
* PDF 报告文件（注意这不应该是notebook的导出，请按照[模板](https://github.com/nd009/capstone/blob/master/capstone_report_template.md)填写）
* 项目相关代码

* 包含使用的库，机器硬件，机器操作系统，训练时间等数据的 README 文档

* 你的最优提交分数需要达到kaggle private leaderboard 的top 20%,对于该题目的就是660th/3307,对应logloss得分为0.18267

* 符合Udacity的[项目要求](https://review.udacity.com/#!/rubrics/273/view)。




