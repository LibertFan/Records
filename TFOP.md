# 1.Tensorflow 如何自定义初始化方式？
 
我们企图不使用 tf.global_variables_initializer 这个命令来对所有的参数进行初始化。

因为有些情况下，我们的参数初始化是不支持并行的，也就是说我们的参数初始化之间是有依赖的，我们企图解决这个问题。

# 2.Tensorflow 的容器 tf.GraphKeys.GLOBAL_VARIABLES 到底是什么样的collection？

2.1. tf.GraphKeys.GLOBAL_VARIABLES 可以在多台设备上共享，
tf.GraphKeys.TRAINABLE_VARIABLES 是tensorflow用来计算梯度的变量，与trainable=True 是一样的效果。
tf.GraphKeys.LOCAL_VARIABLES 是不用计算梯度，也就是说维持变量不变，与 trainable=False 是一样的效果。

2.2. 我们可以通过 tf.add_to_collections 来自定义容器
如何在batchnorm的时候来自定义容器？（去看 tensorflow 的 batch_norm 的源代码）

2.3. 获得在 scope 下已经定义好的变量
我们可以使用tf.get_variable, 同时设置reuse=True，就可以拿到我们在这个scope下定义的变量？（这个功能是不是有些鸡肋？）

# 3.

