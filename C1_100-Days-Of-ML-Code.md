# 原文来自：[Avik-Jain/100-Days-Of-ML-Code](https://github.com/Avik-Jain/100-Days-Of-ML-Code/blob/master/Code/Day3_Multiple_Linear_Regression.md)

# 多远线性回归


<p align="center">
  <img src="https://github.com/Avik-Jain/100-Days-Of-ML-Code/blob/master/Info-graphs/Day%203.jpg">
</p>


## 第一步：数据预处理

### 导入相关库文件
```python
import pandas as pd
import numpy as np
```
### 导入训练数据集
```python
dataset = pd.read_csv('50_Startups.csv')
X = dataset.iloc[ : , :-1].values
Y = dataset.iloc[ : ,  4 ].values
```

### 对多样性数据进行编码
```python
from sklearn.preprocessing import LabelEncoder, OneHotEncoder
labelencoder = LabelEncoder()
X[: , 3] = labelencoder.fit_transform(X[ : , 3])
onehotencoder = OneHotEncoder(categorical_features = [3])
X = onehotencoder.fit_transform(X).toarray()
```

### 避免虚拟变量陷阱
```python
X = X[: , 1:]
```

### 将数据集划分为训练数据集和测试数据集
```python
from sklearn.cross_validation import train_test_split
X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size = 0.2, random_state = 0)
```
## 第二步：使用多远线性回归去进行训练的配置
```python
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train, Y_train)
```

## 第三步：取得预言测试数据的结果
```python
y_pred = regressor.predict(X_test)
```
