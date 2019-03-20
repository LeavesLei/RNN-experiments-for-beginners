## Task 5: Sequence to sequence (Addition)
- Goal:输入是形如'854+376'（'458+673'的倒序），结果（label）为'1131'。使用RNN网络来识别：sequence2sequence
- 数据的生成可以稍微看下，不是重点
- 重点是这部分的RNN结构，与前几个实验的RNN结构都不一样。先了解处理seq2seq文件的Encoder-Decoder模型。这篇文章讲了Encoder-Decoder基本实现，讲得还可以：[seq2seq 的 keras 实现](https://www.jianshu.com/p/c294e4cb4070)关注model.add(layers.RepeatVector(DIGITS + 1))与model.add(layers.TimeDistributed(layers.Dense(len(chars))))。思考为什么要加上这两句。

#### TIPS
- 可以使用model.summary()打印出网络结构与参数数量，自己推一下。
- 关注参数return_sequences（默认为False）。思考为什么有时候要置为True。

#### 相关论文
- [Learning to Execute](http://arxiv.org/abs/1410.4615)   进一步了解此task
- [Sequence to Sequence Learning with Neural Networks](http://papers.nips.cc/paper/5346-sequence-to-sequence-learning-with-neural-networks.pdf)    进一步了解seq2seq
