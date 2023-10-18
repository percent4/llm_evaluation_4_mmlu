## 数据集

**MMLU**（Massive Multitask Language Understanding）数据集下载：

[MMLU数据集下载](https://people.eecs.berkeley.edu/~hendrycks/data.tar)

## 评估结果

运行方式：

```bash
python3 evaluate_hf.py -m /workspace/models/llama2-7b-hf
```
具体结果参考results文件夹

### LLAMA-2评估

| 模型尺寸        | Average weighed accuracy | STEM   | humanities | social sciences | other  | Inference Time(s) |
| ----------- | ------------------------ | ------ | ---------- | --------------- | ------ | ----------------- |
| llama-2-7b  | 0.4596                   | 0.3704 | 0.4338     | 0.5184          | 0.5244 | 2468.45           |
| llama-2-13b | 0.5568                   | 0.4427 | 0.5443     | 0.6341          | 0.6076 | 4123.48           |
| llama-2-70b | 0.6911                   | 0.5779 | 0.6516     | 0.8044          | 0.7461 | 14961.76          |

### 其它模型评估

| 模型                 | Average weighed accuracy | STEM   | humanities | social sciences | other  | Inference Time(s) |
| ------------------ | ------------------------ | ------ | ---------- | --------------- | ------ | ----------------- |
| Baichuan-7B        | 0.4261                   | 0.3615 | 0.3853     | 0.4927          | 0.4821 | 3620.22           |
| Baichuan2-7B-Base  | 0.5431                   | 0.4463 | 0.5133     | 0.6126          | 0.6104 | 3742.95           |
| Baichuan2-13B-Base | 0.5901                   | 0.4954 | 0.5505     | 0.6783          | 0.6521 | 3460.3            |
| internlm-20b       | 0.6063                   | 0.5113 | 0.5615     | 0.7033          | 0.6675 | 5709.98           |
| Mistral-7B-v0.1    | 0.6267                   | 0.5268 | 0.5658     | 0.7364          | 0.7039 | 2517.74           |


![](https://s2.loli.net/2023/10/18/3FJk2psOInuTAZ9.png)

![](https://s2.loli.net/2023/10/18/tjZrMLHk3cOmfVs.png)

## 参考网址

*   [mmlu](https://github.com/ollmer/mmlu)
*   [test](https://github.com/hendrycks/test)
*   [OpenCompass MMLU](https://opencompass.org.cn/dataset-detail/MMLU)
