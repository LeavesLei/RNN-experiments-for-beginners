## RNN-experiments-for-beginners
#### If you want the English edition, please go [here](https://upc-mai-dl.github.io/rnn-lab-guided/).
在UPC-FIB交流期间选了Deep Learning这门课，课上有关于RNN的内容与实验。正好自己之前也没接触过RNN，正好将课上的一些RNN实验整理一下。RNN部分的授课老师是[Javier Bejar](bejar@cs.upc.edu)先生，此仓库已得到Bejar的授权，实验源码也出自Bejar之手，自己编写了ipynb文件用以熟悉实验的具体步骤（特别是数据集部分）。

- **英文实验说明：[ guided laboratory of the RNN topic](https://upc-mai-dl.github.io/rnn-lab-guided/)** （懒得翻译...所以强烈建议看看原版实验说明）
- 如何使用此repository？ 刷一遍RNN（Basic RNN，LSTM，GRU等）的理论，就可以使用来做这里面的实验了。
- 如果你觉得哪里写得不够清楚，或者有问题，请告诉我[leishiye@gmail.com](leishiye@gmail.com). 毕设闲暇之余弄的这个repo，很多地方只写了个大概
- 具体实验说明还未翻译，如果有NLP爱好者且有余力，欢迎完善此仓库，联系方式同上

## How to Use?
repo中一共有5个基本的RNN实验（数据集已经包括在内，无需单独下载），涵盖了以下几个基本方面：
- [Time series prediction as regression](https://github.com/LeavesLei/RNN-experiments-for-beginners/tree/master/AirQuality)
- [series prediction as classification](https://github.com/LeavesLei/RNN-experiments-for-beginners/tree/master/Electric)
- [Sentiment analysis](https://github.com/LeavesLei/RNN-experiments-for-beginners/tree/master/Sentiment)
- [Text generation as character level prediction](https://github.com/LeavesLei/RNN-experiments-for-beginners/tree/master/TextGeneration)
- [Sequence to sequence prediction](https://github.com/LeavesLei/RNN-experiments-for-beginners/tree/master/Seq2seq)

建议先运行Knowing_dataset.ipynb文件了解数据集结构。然后运行.py开始训练。
## Some confusion I had met
- LSTM中lag代表什么？ lag代表输入的数量。例如用前6天的天气预测当天的天气，那么lag=6（前6天的天气），ahead=1（当天的天气）。若预测今明两天的天气，则ahead=2。
- Keras中LSTM的输入尺寸：(batch_size, timesteps, input_dim)
- **强烈建议！！！** 动手推一遍LSTM的参数数量对于理解网络结构十分有好处[Keras关于LSTM的units参数，还是不理解? - Scofield的回答 - 知乎](https://www.zhihu.com/question/64470274/answer/497314160). 
- 如何查看自己搭建的RNN网络结构：**model.summary()** 会自动打印出来。

## References
- https://keras.io/zh/layers/recurrent/


### If the repository ha help you, just give me a smile:)
