<!--
 * @Author: liubeiming
 * @Date: 2023-03-21 10:12:22
-->
# alpaca_chinese_dataset

**鲁迅说过：有多少人工，才有多少智能**

当前的聊天对话模型数据集主要都是由英文构成，但是当前中文聊天模型构建的需求也较为迫切，因此我们将斯坦福的alpaca数据集进行中文翻译，并再制造一些对话数据，并开源提供。

我们发现翻译API的效果不如chatGPT，因此我们现在将切分成17份的数据集使用chatGPT替代了使用翻译API进行翻译。

此翻译并非完全的chatgpt机翻，会进行人工校验，遇到英文特异性表达的时候会变为较为中文化的表述，因此每日翻译量有限。

遇到完全不能翻译为中文的数据，可能会跳过，因此这将不是一个纯中文或中文--英文数据集。可能不适合拿来做翻译相关训练

分配下去的数据集应该能够确保全部翻译，预计alpaca每日增量约2500行，额外的非alpaca中文数据集我们预计也会以工作日120条左右的速度增加记录，预计每天会500行左右的数据

## 目前数据集认领情况：

- 阿扣扣 清华大学工工（alpaca_data-0-3252-英文）
- 黄堃淏 电子科大软院（alpaca_data-3252-6382-英文）
- 焦丽华 电子科大软院（alpaca_data-6382-9407-英文）
- 何余晨 电子科大软院（alpaca_data-9407-12345-英文）
- 张瑞钦 电子科大软院（alpaca_data-12345-15323-英文）
- 梁渊 电子科大软院（alpaca_data-15323-18280-英文）
- 王银杉 电子科大软院（alpaca_data-18280-21320-英文）
- 其他数据集当前暂无人认领，等待我们之前的数据标记完或者其他小伙伴认领～

## 额外数据集

- 阿扣扣（企业管理问题、三国问题）
- 黄堃淏 电子科大软院（名词解释类问题）
- 焦丽华 电子科大软院（党建类数据集）
- 何余晨 电子科大软院（建议类数据集）
- 张瑞钦 电子科大软院（历史类数据集）
- 梁渊 电子科大软院（学习类数据集）
- 王银杉 电子科大软院（科技类数据集）


## DOING

- 加入除了alpaca之外的其他中文聊天对话
- 人工微调，部分并不中文化的问题，我们将重新询问chatgpt或文心一言，重新获取回答并覆盖掉alpaca的回答

## 其他数据集
- chatglm问题数据集：针对chatglm中我们发现的问题，使用文心一言或chatgpt进行回答，并重新收录
