<!-- ELUCENIA technical documentation · fib-4 · ja · no clinical/professional/rights approval -->

# FIB-4（肝線維化）

[条件・出典・許諾](https://elucenia.org/ja/tools/fib-4)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 年齢

`idade`

年 · 範囲: 18–100

### AST

`ast`

U/L · 範囲: 1–5000

### ALT

`alt`

U/L · 範囲: 1–5000

### 血小板

`plq`

× 10³/mm³ · 範囲: 5–1500

### 状況

`etio`

- `masld` — 脂肪化（MASLD/NAFLD）
- `viral` — C型肝炎またはHIV/HCV

## 方法の版

FIB-4/Sterling 2006；HCV/HIV閾値1.45/3.25に対しMASLD 1.3/2.67，≥65歳2.0

## 記載された計算式

FIB-4 = (年齢 × AST) ÷ (血小板 \[10⁹/L\] × √ALT)。

MASLD： \< 1.30は進行線維化を除外（65歳以上では\< 2.0）；\> 2.67は進行線維化を示唆。C型肝炎/HIV： \< 1.45および\> 3.25。

## 限界・対象集団

Sterling 2006のFIB-4はHIV/HCV共感染の患者で開発され、Ishak 4–6の線維化に対して\<1.45と\>3.25の閾値が評価されました。式には年単位の年齢、U/L単位のAST・ALT、10^9/L単位の血小板を用います。これらの閾値と原集団をMASLDの基準や年齢調整と自動的に置き換えることはできず、その変法には専用の出典が必要です。

## 参考文献

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

進行した線維化の可能性が低い（FIB-4 < 1.30）


### 2

判定不能の結果：エラストグラフィーを追加する


### 3

判定不能の結果：エラストグラフィーを追加する


### 4

判定不能の結果：エラストグラフィーを追加する

65歳以上（DHGNA/MASLD）では、使用される下限カットオフは 2,0 です。


### 5

進行した線維化の可能性が高い（FIB-4 > 2.67）

