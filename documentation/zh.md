<!-- ELUCENIA technical documentation · nrs-2002 · zh · no clinical/professional/rights approval -->

# NRS-2002

[条件、来源与许可](https://elucenia.org/zh/tools/nrs-2002)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 营养状态受损

`estado`

- `0` — 无：营养状况正常
- `1` — 轻度：3个月内体重下降\>5%，或过去一周摄入为需要量的50至75%
- `2` — 中度：2个月内下降\>5%，或BMI 18.5至20.5且一般状况受损，或摄入25至60%
- `3` — 重度：1个月内下降\>5%（3个月内\>15%），或BMI\<18.5且一般状况受损，或摄入0至25%

### 疾病严重程度（需求增加）

`gravidade`

- `0` — 无：营养需求正常
- `1` — 轻度：髋部骨折、慢性病伴急性并发症（肝硬化、COPD、血液透析、糖尿病、癌症）
- `2` — 中度：重大腹部手术、卒中、重症肺炎、血液肿瘤
- `3` — 重度：头部外伤、骨髓移植、ICU且APACHE II\>10

### 年龄 ≥ 70 岁

`idade`

## 方法版本

NRS 2002/ESPEN Kondrup 2003：2领域0–3，年龄≥70加1，总分0–7

## 已记录的公式

评分=营养状态受损（0–3）+疾病严重程度（0–3）+年龄≥70岁时加1分。总分0–7。

评分≥3：营养风险。

## 限制与适用人群

NRS-2002是结合营养状态与疾病严重程度的风险筛查。其开发区分了较可能获益的研究人群；总分不能保证个体反应，也不规定营养支持途径或剂量。定义、适用资格及年龄应与版本一致。

## 参考文献

- [Kondrup J et al. Nutritional risk screening (NRS 2002): a new method based on an analysis of controlled clinical trials. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(02)00214-5)

- [Kondrup J et al. ESPEN guidelines for nutrition screening 2002. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(03)00098-0)

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
