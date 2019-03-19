## Task 2: Time Series Classification (Electric Devices classification )
- Goal: 根据一天中不同时间段的用电量判断是哪种电器

### Dataset
- 输入序列长度为96（每隔15min测一次电器的用电量，15min×4×24=96），然后预测这个电器是
computer/television, dishwasher, fridge, heater, kettle, oven and washing machine
中的哪种（共有七类）
- 说得再详细也只比不上亲自动手。所以请按照[Knowing_dataset.ipynb](https://github.com/LeavesLei/RNN-experiments-for-beginners/blob/master/Electric/Knowing_dataset.ipynb)逐步操作来了解数据集

### 网络结构
Power Consumption(INPUT) ——> RNN ——> RNN ——> Dense ——> Class(OUTPUT)
