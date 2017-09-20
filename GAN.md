# 1. GAN in MNIST

## 1.1 GAN论文

(1) 意图模拟真实数据的分布，通过不断地区分真实数据和生成的数据，指导生成的数据向真实的数据靠近。

(2) GAN的结构为什么可以保证生成的数据可以足够贴近真是的数据：
  
    模型的 Loss Function 如下所示：
    
    $$ \min_{G}\max_{D}V(G,D)=\mathbb{E}_{x\sim P_{data}}log\big(D(x)\big)+ \mathbb{E}_{x\sim P_{\mathbf{z}}(z)}\big(1-D\big(G(x)\big)\big)$$
 
    整个模型的 Loss Function 会在真实数据的分布和生成数据的分布相同的时候达到最大值。
    
    所以只要保证模型能够优化到全局最小值，就可以达到我们想要的效果。

(3) GAN在训练初期训练困难，这是因为


## 1.2 在Mnist数据集上的实现

## 1.3 反思

# 2.  

# 3

# 4
