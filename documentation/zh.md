<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · zh · no clinical/professional/rights approval -->

# 高血糖时校正钠

[条件、来源与许可](https://elucenia.org/zh/tools/sodio-corrigido-hiperglicemia)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 实测钠

`na`

mEq/L · 范围: 100–180

### 血糖

`glic`

mg/dL · 范围: 50–2000

## 方法版本

Katz 1973系数1.6、Hillier 1999系数2.4，每超出100的100 mg/dL葡萄糖

## 已记录的公式

Hillier: 校正Na = Na + 2.4 × (葡萄糖 − 100) ÷ 100.

Katz: 校正Na = Na + 1.6 × (葡萄糖 − 100) ÷ 100.

## 限制与适用人群

Hillier 1999在六名健康受试者中研究诱导的急性高血糖。钠与葡萄糖的关系非线性，尤其在400 mg/dL以上；平均系数2.4并不能对全部人群及浓度提供普遍精确的描述。Katz 1.6和Hillier 2.4是不同变体，分开展示。校正钠是估计值，不是保证的未来测量值，也不是校正速度处方。

## 参考文献

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

校正钠正常：测得的低钠血症由葡萄糖所致（水移位）

| 结果详情 | |
| --- | --- |
| 校正钠（Katz，1,6） | 138.0 mEq/L |


### 2

即使校正后仍为真性低钠血症

| 结果详情 | |
| --- | --- |
| 校正钠（Katz，1,6） | 131.2 mEq/L |


### 3

校正钠升高：存在游离水缺乏

| 结果详情 | |
| --- | --- |
| 校正钠（Katz，1,6） | 153.2 mEq/L |

