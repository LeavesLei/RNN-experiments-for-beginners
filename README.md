# RNN-experiments-for-beginners
- If you want the English edition, please go to [here](https://upc-mai-dl.github.io/rnn-lab-guided/).
- 在UPC-FIB交流期间选了Deep Learning这门课，课上有关于RNN的内容与实验。正好自己之前也没接触过RNN，正好将课上的一些RNN实验整理一下。

## Some confusion I had met
- LSTM中lag代表什么？ lag代表输入的数量。例如用前6天的天气预测当天的天气，那么lag=6（前6天的天气），ahead=1（当天的天气）。若预测今明两天的天气，则ahead=2。
- Keras中LSTM的输入尺寸：(batch_size, timesteps, input_dim)


## References
- https://keras.io/zh/layers/recurrent/


### If the repository have help you, just give me a smile😀
