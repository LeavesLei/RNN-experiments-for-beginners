## Task 5: Sequence to sequence (Addition)
- Goal:输入是形如'854+376'（'458+673'的倒序），结果（label）为'1131'。使用RNN网络来识别：sequence2sequence
- 数据的生成可以稍微看下，不是重点
- 重点是这部分的RNN结构，与前几个实验的RNN结构都不一样。关注model.add(layers.RepeatVector(DIGITS + 1))
与model.add(layers.TimeDistributed(layers.Dense(len(chars))))。思考为什么要加上这两句。

#### TIPS
- 可以使用model.summary()打印出网络结构与参数数量，自己推一下。
- 关注参数return_sequences（默认为False）。思考为什么有时候要置为True。
