---
layout:     post
title:      读书笔记-Tensor实战Google深度学习框架
category: 读书笔记
description: 读书笔记
tags: AI
---

# 第1章 深度学习简介 
## 1.1 人工智能、机器学习与深度学习
- 机器学习定义： T E P 如果一个程序可以在任务T上，随着经验E的增加，效果P也可以随之增加，则称这个程序可以从经验中学习。

- 对于机器学习问题来说，特征提取不是一件简单的事情
- 深度学习解决的核心问题之一就是自动地将简单的特征组合成更加复杂的特征，并使用这些组合特征解决问题。
- 小白鼠实验说明，虽然哺乳动物大脑分成了很多区域，但这些区域得学习机制却是相似的。
- 现代深度学习并不拘泥于模拟人脑神经元和人脑得工作机理。
- 现代深度学习已经超越了神经科学观点。<br>

![](images/2018-1-8-TensorFlow/1.jpg)

## 1.2 深度学习的发展历程
- 1943年，McCulloch-Pitts结构，缺点：通过人类经验设置

- 1958年 感知机模型 McCulloch-Pitts结构和感知机模型极大地影响了现代机器学习 缺点：只能解决线性问题，无法解决异或问题。在当时的计算能力下，实现多层神经网络是不可能的事

- 20世纪80年代末，分布式知识表达，神经网络反向传播算法的提出，分布式知识表达，让神经网络从宽带的方向走向了深度的方向。

- 80年代末，90年代初，提出卷积神经网络和循环神经网络，LSTM，直到今天LSTM仍是主流。

- 98年，在神经网络发展的同时，SVM

- 2010年，云计算->深度神经网络

## 1.3 深度学习的应用
### 1.3.1 计算机视觉
- ImageNet数据集，深度学习不仅突破了图像分类的技术瓶颈，也突破了物体识别得技术瓶颈
- 工业领域，谷歌无人驾驶车，youtubu，谷歌地图，谷歌图像搜索，人脸识别，光学字符识别

### 1.3.2 语音识别
- TIMIT数据集
- 工业界，谷歌的Google Now， 苹果的Siri，微软的Xbox和Skype

### 1.3.3 自然语言处理
- 单词向量
- 机器翻译
- 情感分析
### 1.3.4 人机博弈
- AlphaGo

## 1.4 深度学习工具介绍和对比

# 第2章 TensorFlow环境搭建
## 2.1 TensorFlow的主要依赖包
### 2.1.1 Protocol Buffer
### 2.1.2 Bazel
### 2.2 TensorFlow安装
### 2.2.1 使用Docker安装
### 2.2.2 使用pip安装
### 2.2.3 从源代码编译安装
## 2.3 TensorFlow测试样例

# 第3章 TensorFlow入门
## 3.1 TensorFlow计算模型——计算图
- TensorFlow是一个通过计算图的形式来表述计算的编程系统。TF的每一个计算都是计算图上的一个节点，而节点之间的边描述了计算之间的依赖关系。
- 通过tf.Graph函数来生成新的计算图。
- TensorFlow中的计算图不仅仅可以用来隔离张量和计算，它还提供了管理张量和计算的机制。
- tf.Graph.device指定运行计算的设备。
- 通过集合管理不同的资源。

## 3.2 TensorFlow数据模型——张量
### 3.2.1 张量的概念
- 从功能角度，张量可以被简单理解为多维数组。
- 在张量中并没有真正保存数字，它保存的是如何得到这些数字的计算过程。
- 张量有3个属性：

### 3.2.2 张量的使用 
## 3.3 TensorFlow运行模型——会话
##3.4 TensorFlow实现神经网络
### 3.4.1 TensorFlow游乐场及神经网络简介
### 3.4.2 前向传播算法简介
### 3.4.3 神经网络参数与TensorFlow变量
### 3.4.4 通过TensorFlow训练神经网络模型
### 3.4.5 完整神经网络样例程序 

# 第4章 深层神经网络 
## 4.1 深度学习与深层神经网络 
### 4.1.1 线性模型的局限性 
### 4.1.2 激活函数实现去线性化
### 4.1.3 多层网络解决异或运算
## 4.2 损失函数定义
### 4.2.1 经典损失函数
### 4.2.2 自定义损失函数
## 4.3 神经网络优化算法
## 4.4 神经网络进一步优化
### 4.4.1 学习率的设置
### 4.4.2 过拟合问题
### 4.4.3 滑动平均模型

# 第5章 MNIST数字识别问题
## 5.1 MNIST数据处理
## 5.2 神经网络模型训练及不同模型结果对比
### 5.2.1 TensorFlow训练神经网络
### 5.2.2 使用验证数据集判断模型效果
### 5.2.3 不同模型效果比较
## 5.3 变量管理
## 5.4 TensorFlow模型持久化
### 5.4.1 持久化代码实现
### 5.4.2 持久化原理及数据格式
## 5.5 TensorFlow最佳实践样例程序

# 第6章 图像识别与卷积神经网络 
## 6.2 卷积神经网络简介 
## 6.3 卷积神经网络常用结构 
### 6.3.1 卷积层
### 6.3.2 池化层
## 6.4 经典卷积网络模型
### 6.4.1 LeNet-5模型
### 6.4.2 Inception-v3模型
## 6.5 卷积神经网络迁移学习 
### 6.5.1 迁移学习介绍 
### 6.5.2 TensorFlow实现迁移学习 

第7章 图像数据处理 170
7.1 TFRecord输入数据格式 170
7.1.1 TFRecord格式介绍 171
7.1.2 TFRecord样例程序 171
7.2 图像数据处理 173
7.2.1 TensorFlow图像处理函数 174
7.2.2 图像预处理完整样例 183
7.3 多线程输入数据处理框架 185
7.3.1 队列与多线程 186
7.3.2 输入文件队列 190
7.3.3 组合训练数据（batching） 193
7.3.4 输入数据处理框架 196
小结 198
第8章 循环神经网络 200
8.1 循环神经网络简介 200
8.2 长短时记忆网络（LTSM）结构 206
8.3 循环神经网络的变种 212
8.3.1 双向循环神经网络和深层循环神经网络 212
8.3.2 循环神经网络的dropout 214
8.4 循环神经网络样例应用 215
8.4.1 自然语言建模 216
8.4.2 时间序列预测 225
小结 230
第9章 TensorBoard可视化 232
9.1 TensorBoard简介 232
9.2 TensorFlow计算图可视化 234
9.2.1 命名空间与TensorBoard图上节点 234
9.2.2 节点信息 241
9.3 监控指标可视化 246
小结 252
##第10章 TensorFlow计算加速
##10.1 TensorFlow使用GPU
##10.2 深度学习训练并行模式 
##10.3 多GPU并行
##10.4 分布式TensorFlow 
###10.4.1 分布式TensorFlow原理 
###10.4.2 分布式TensorFlow模型训练 
###10.4.3 使用Caicloud运行分布式TensorFlow 
##小结