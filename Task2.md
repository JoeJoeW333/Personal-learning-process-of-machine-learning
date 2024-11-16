# Task 2

## 2.1 随记

### 一元线性回归

1. 算法原理：取所有样本点到该线性模型的距离之和（预测误差）最短的模型为最优

2. 算法模型总结：

   | 单一客观变量                   | f(x)=w1x1+b                          |
   | ------------------------------ | ------------------------------------ |
   | 单一二值变量（是否）           | f(x)=w1x1+w2x2+b                     |
   | 有序多值离散变量（大中小）     | f(x)=w1x1+w2x2+w3x3+b                |
   | 无序多值离散变量（肤色黄黑白） | f(x)=w1x1+w2x2+w3x3+w4x4+w5x5+w6x6+b |

   其中无序多值离散变量等同于二值变量+多值离散变量，也就是一个人黄不黄、白不白、黑不黑各自是和否的6个权重

3. 最小二乘估计：用均方误差最小来求解损失函数

4. 最大似然估计：用来估计概率分布的参数值。对随机变量建立模型之前要求确定概率分布模型，因此最大似然估计首先确定是什么分布，然后根据分布类型求概率分布，然后取联合概率最大的为概率的估计值。（写出随机变量的概率密度函数-》写似然函数-》求实际概率的估计值）

5. 求解W和B：转化成多元函数求最值点的问题，更具体来说是凸函数求最值

6. 梯度（多元函数的一阶导数），分别就n元函数对自变量的各个x变量求偏导

7. hessian（海塞）矩阵：多元函数的二阶导数，也就是就n元函数对自变量的各个x变量求二阶偏导

8. 半定正矩阵：实对称矩阵的所有顺序主子式均为肺腑

9. 机器学习三要素：模型（确定假设空间）、策略（确定评价标准、产出损失函数）、算法（求解损失函数、确定最优模型）

10. 常用：梯度下降法、牛顿法



### 多元线性回归

求解W是多元函数求解最值的 问题，也是凸函数求最值的问题：

- 证明凸函数存在
- 用凸函数求最值的方式求解出W



 