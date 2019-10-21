# SparkMLlib
### 目标
实现Codeforces 推荐系统

### 数据准备
从Codeforces中将用户所有的提交记录全部爬取，然后每一个用户每一道题目计算AC_Rate,得到如下表
![tou.png](https://i.loli.net/2019/10/21/pvS8yWlBRQ3zabC.png)


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
