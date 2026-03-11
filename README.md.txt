# 电商用户流失预测项目

## 项目背景
随着电商行业竞争加剧，用户流失成为核心运营指标。本项目基于用户历史行为数据，构建分类模型预测高流失风险用户。

## 数据集说明
来源：https://www.kaggle.com/datasets/kartikeybartwal/ecommerce-product-recommendation-collaborative
字段：14个
样本量：1000条

## 分析方法
1. 数据清洗：处理缺失值、异常值
2. 特征工程：构造 RFM 特征
3. 建模对比：逻辑回归、随机森林
4. 评估指标：召回率、AUC曲线

## 主要结论
1. 特征重要性最高的前几位是 收入，总支出，平均订单价值
2. 随机森林的 AUC 达到 0.5409 ，说明模型不能较好地区分流失与留存用户。原因可能有特征与标签的弱相关性，只有1000条数据，数据量不足等

## 文件结构
- `churn_analysis.ipynb`：完整分析代码
- `user_personalized_features.csv`：原始数据
- `README.md`：项目说明