# SparkMLlib

## Codeforces 推荐系统

### 目标
实现Codeforces 推荐系统  
根据用户的提交记录对用户的水平进行评估，然后为用户推荐适合其水平的题目

### 数据准备
从Codeforces中将用户所有的提交记录全部爬取，然后每一个用户每一道题目计算AC_Rate,得到如下表
![tou.png](https://i.loli.net/2019/10/21/pvS8yWlBRQ3zabC.png)  
以AC_Rat代表用户的能力  
后期改进：由于简单题用户基本都是一次提交就能通过，并不能很好的体现用户的水平

### 环境准备
1. Spark集群搭建
2. jupyter notebook

### 步骤
1. 对数据划分训练集和测试集
2. 使用ALSModel 在训练集上训练出模型
3. 使用 RegressionEvaluator 进行模型评估
4. 对用户进行推荐

### 结果展示
*模型评估*
![pinggu.png](https://i.loli.net/2019/10/21/dzKAfJQI1ktuVyT.png)
*对用户进行推荐*
![recom.png](https://i.loli.net/2019/10/21/TEy2IDlxOmCJV4B.png)

## 短信分类

### 目标
使用SparkMLlib 对短信进行分类

### 数据准备
使用 SMSSpamCollection 数据集

### 环境准备
1. Spark集群搭建
2. jupyter notebook

### 步骤
1. 对数据划分训练集和测试集
2. 使用 Word2Vec 将短信文本转化成数值型词向量
3. 使用 MultilayerPerceptronClassifier 训练一个多层感知模型
4. 使用 Pipeline 对数据进行处理和模型的训练
5. 使用模型对测试数据进行分类处理
6. 测试数据集上测试模型的预测精确度
### 结果展示
![res.png](https://i.loli.net/2019/10/21/bVWOZB2aQYNI1sP.png)
![accuracy.png](https://i.loli.net/2019/10/21/i1QMoknfJCdj38F.png)

finished

