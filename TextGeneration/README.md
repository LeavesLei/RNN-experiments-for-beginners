## Task 4: Sequence Classification (Text Generation)
Note: 这个实验有可能出现OOM（out of memory）错误，是由于机器性能不足导致。两个解决办法：
1. 优化代码
2. 换台机器

- Goal：通过RNN网络学习多首诗，来预测一句诗的下一个字母（letter）是什么
- [TextGenerator.py](https://github.com/LeavesLei/RNN-experiments-for-beginners/blob/master/TextGeneration/TextGenerator.py)训练模型以及预测
- [GenPeotry.py](https://github.com/LeavesLei/RNN-experiments-for-beginners/blob/master/TextGeneration/GenPoetry.py)根据TextGenerator生成的模型随机生成一首诗
- 同理：重点关注数据清洗工作。
