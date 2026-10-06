<!-- ELUCENIA technical documentation · fib-4 · zh · no clinical/professional/rights approval -->

# FIB-4（肝纤维化）

[条件、来源与许可](https://elucenia.org/zh/tools/fib-4)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 年龄

`idade`

年 · 范围: 18–100

### AST

`ast`

U/L · 范围: 1–5000

### ALT

`alt`

U/L · 范围: 1–5000

### 血小板

`plq`

× 10³/mm³ · 范围: 5–1500

### 适用情境

`etio`

- `masld` — 脂肪变（MASLD/NAFLD）
- `viral` — 丙型肝炎或HIV/HCV

## 方法版本

FIB-4/Sterling 2006；HCV/HIV阈值1.45/3.25，对比MASLD 1.3/2.67和≥65岁2.0

## 已记录的公式

FIB-4 = (年龄 × AST) ÷ (血小板 \[10⁹/L\] × √ALT)。

MASLD： \< 1.30排除进展期纤维化（65岁起\< 2.0）；\> 2.67提示进展期纤维化。丙肝/HIV： \< 1.45及\> 3.25。

## 限制与适用人群

Sterling 2006的FIB-4在HIV/HCV共感染患者中开发，针对Ishak 4–6级纤维化评估了\<1.45和\>3.25阈值。公式使用以年计的年龄、以U/L计的AST及ALT，以及以10^9/L计的血小板。这些阈值及原始人群不能自动与MASLD标准或年龄调整互换；这些变体需要各自的来源。

## 参考文献

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

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

进展期纤维化概率低（FIB-4 < 1.30）


### 2

结果不确定：补充弹性成像


### 3

结果不确定：补充弹性成像


### 4

结果不确定：补充弹性成像

从 65 岁起（DHGNA/MASLD），所用的下限截点为 2,0。


### 5

进展期纤维化概率高（FIB-4 > 2.67）

