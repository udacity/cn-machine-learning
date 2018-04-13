# 算式识别

## AWS

由于此项目要求的计算量较大，建议使用亚马逊 p3.2xlarge 云服务器来完成该项目，在使用 p3 之前，你可以先用 p2.xlarge 练手，参考：[在aws上配置深度学习主机 ](https://zhuanlan.zhihu.com/p/25066187)，[利用AWS学习深度学习](https://zhuanlan.zhihu.com/p/33176260)。

## 描述

使用深度学习识别一张图片中的算式。

* 输入：一张彩色图片
* 输出：算式的内容

## 数据

数据集可以通过这个链接下载：

[https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd009/MLND+Capstone/Mathematical_Expression_Recognition_train.zip](https://s3.cn-north-1.amazonaws.com.cn/static-documents/nd009/MLND+Capstone/Mathematical_Expression_Recognition_train.zip)

此数据集包含10万张图片，每张图里面都有一个算式。

* 可能包含 `+-*` 三种运算符
* 可能包含一对括号，也可能不包含括号
* 每个字符都可能旋转，所以 `+` 号可能长得像我们平时手写的 `*` 号，不过 `*` 号有六个瓣

![](example.jpg)

## 建议

建议使用 OpenCV, tensorflow, Keras 完成该项目。其他的工具也可以尝试，比如 pytorch, mxnet 等。

* [OpenCV 项目](https://github.com/opencv/opencv)
* [tensorflow 项目主页](https://github.com/tensorflow/tensorflow)
* [Keras 项目主页](https://github.com/fchollet/keras)
* [OpenCV python tutorials](https://docs.opencv.org/master/d6/d00/tutorial_py_root.html)
* [Keras 英文文档](https://keras.io)
* [Keras 中文文档](https://keras.io/zh/)

### 建议模型

如果你不知道如何去构建你的模型，可以看看下面的论文：

[An End-to-End Trainable Neural Network for Image-based Sequence Recognition and Its Application to Scene Text Recognition](https://arxiv.org/abs/1507.05717)

## 最低要求

本项目的最低要求是99%的准确率。

## 应用(可选)(推荐)

为了能够让他人使用此 OCR 服务，我们可以将模型部署到服务器上。

### 网页应用

推荐的工具：

* [Flask](https://github.com/pallets/flask)
* [Flask 中文文档](http://docs.jinkan.org/docs/flask/)

## 评估

你的项目会由优达学城项目评审师依照[机器学习毕业项目要求](https://review.udacity.com/#!/rubrics/1785/view)来评审。请确定你已完整的读过了这个要求，并在提交前对照检查过了你的项目。提交项目必须满足所有要求中每一项才能算作项目通过。

## 提交

* PDF 报告文件
* 所有代码文件（jupyter notebook）
* 以上 notebook 导出的 html 文件
* 包含使用的库，机器硬件，机器操作系统，训练时间等数据的 README 文档（使用 Markdown 编写）
