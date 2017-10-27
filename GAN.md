# 1. GAN in MNIST

## 1.1 GAN论文

(1) 意图模拟真实数据的分布，通过不断地区分真实数据和生成的数据，指导生成的数据向真实的数据靠近。

(2) GAN的结构为什么可以保证生成的数据可以足够贴近真是的数据：
  
模型的 Loss Function 如下所示:
 
$$ \min_{G} \max_{D} V(G,D) = \mathbb{E}_{x\sim P(x)} [log(D(x))] + \mathbb{E}_{x\sim P(x)} [log(D(x))] $$
    
 
为了标记的方便，我们可以将x的真是分布记作$p_{g}(x)$

我们将上面的式子写成积分的形式，那么就可以看到：

$$\int log\big(D(x)\big)p_{data}(x) $$

整个模型的 Loss Function 会在真实数据的分布和生成数据的分布相同的时候达到最大值。

所以只要保证模型能够优化到全局最小值，就可以达到我们想要的效果。

(3) GAN在训练初期训练困难，这是因为


## 1.2 在Mnist数据集上的实现

## 1.3 反思

# 2. Maximum-Likelihood Augmented Discrete Generative Adversial Networks

这里使用的是最优的情况来进行处理的，但是在训练当中我们并不能够保证训练器在初始的 epoch 当中，
并不能够保证分类器已经达到最优。所以我们可以尝试使用的别的来修改这篇文章给出的结论。

# 3. WGAN and WGAN-GP


# 4. GAN 中的问题

1.在训练的过程当中，出现了很多的问题，尤其突出的问题在loss的值总是为 nan， 这样的结果给后面的训练造成了很大的影响。现在我们试图通过
tf.log(tf.maximum(x, 1e-9)) 来在数值上解决这个问题，不过显然这不是长久之计。
