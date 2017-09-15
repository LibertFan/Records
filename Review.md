# 1. 统计学

## 0. 概率的定义

**概率空间：**非空集合$\Omega$为样本空间，事件的全体为事件域，是$\Omega$的一些子集的集合（子集类）。

非空集合$\Omega$的一个子集类$\mathcal{F}$称为$\Omega$上的一个$\sigma$-域，如果：

(1) $\emptyset,\ \Omega \in \mathcal{F}$

(2) $A\in \mathcal{F},\ A^{c} \in \mathcal{F}$

(3) $A_{n} \in \mathcal{F},\ n\geq 1 \Longrightarrow \bigcup_{n}A_{n} \in \mathcal{F}$

$\mathbb{P}$ 被称为概率测度，假如$\Omega$为样本空间，$\mathcal{F}$为$\Omega$上的$\sigma$-域，如果它满足：

(1) 非负性: 对任何$A\in \mathcal{F},\ \mathbb{P}(A)\geq 0$；

(2) 规范性: $\mathbb{P}(\Omega)=1$；

(3) 可列可加性: 对$\mathcal{F}$中互斥的可列个事件$\{A_{n}:n\geq 1\}$， 有：
$$\mathbb{P}(\bigcup_{n\geq 1} A_{n})=\sum_{n\geq 1}\mathbb{P}(A_{n})$$

**随机变量：**概率空间$(\Omega,\ \mathcal{F},\ \mathbb{P})$, $\Omega$为样本空间，$\mathcal{F}$为状态空间，$\mathbb{P}$为概率测度。
$\xi:\ \mathcal{F}\rightarrow \mathbf{R}$是$\Omega$上的函数，称$\xi$为随机变量，如果对于任意$x\in \mathbf{R}$,
$$\{\xi\leq x\}:=\{\omega\in\Omega:\xi(\omega)\leq x\}\in \mathcal{F}$$.

即$\xi$为状态空间$\mathcal{F}$上的可测函数。

**概率分布：**

## 1 不同的收敛的方式

### 1.1 a.s.收敛

P({\omega\in \})

### 1.2 依概率收敛

### 1.3 依分布收敛

### 1.4 平方均值收敛

### 1.5 互相之间的推导关系

## 2 大数定律，中心极限定理

大数定律在方差存在条件下的证明！

中心极限定理是依分布收敛

## 3 回归

### 3.1 线性回归

### 3.2 逻辑回归

## 4 极大似然估计

## 5 Bayes 

### 5.1 Bayes 定理

### 5.2 先验分布与后验分布

另，解释Bayes与线性回归当中参数$p$范数乘法项的关系

## 6



# 2. 机器学习

# 3. 人工智能

## 3.1 搜索算法

### 3.1.1 先深算法

### 3.1.2 先广算法

### 3.1.3 启发式函数

启发式函数的要求：
1.
2.

## 3.2 CSP

## 3.3 Markov

## 3.4 条件随机场？

## 3.5 强化学习
 
### 3.5.1

### 3.5.2 Q-learning

# 4. 概率论

# 5. 时间序列

# 6. 大规模分布式系统？

# 7. 项目相关

## Variatianal Auto-Encoder（给出具体的推导）

## EM算法（与VAE的关系） 

## 人工智能项目描述

### 蒙特卡洛树搜索

### 







