<!-- ELUCENIA technical documentation · sodio-corrigido-hiperglicemia · ja · no clinical/professional/rights approval -->

# 高血糖時の補正ナトリウム

[条件・出典・許諾](https://elucenia.org/ja/tools/sodio-corrigido-hiperglicemia)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 実測ナトリウム

`na`

mEq/L · 範囲: 100–180

### 血糖

`glic`

mg/dL · 範囲: 50–2000

## 方法の版

Katz 1973係数1.6・Hillier 1999係数2.4、100超過の100 mg/dLグルコースごと

## 記載された計算式

Hillier: 補正Na = Na + 2.4 × (グルコース − 100) ÷ 100.

Katz: 補正Na = Na + 1.6 × (グルコース − 100) ÷ 100.

## 限界・対象集団

Hillier 1999は、健康な参加者六人に誘発した急性高血糖を研究しました。ナトリウムとグルコースの関係は非線形で、特に400 mg/dLを超える場合に顕著でした。平均係数2.4は、全ての集団と濃度を普遍的に正確に記述するものではありません。Katz 1.6とHillier 2.4は別の変法で、分けて表示されています。補正ナトリウムは推定であり、保証された将来の測定値でも、補正速度の処方でもありません。

## 参考文献

- [Katz MA. Hyperglycemia-induced hyponatremia: calculation of expected serum sodium depression. N Engl J Med, 1973.](https://doi.org/10.1056/NEJM197310182891607)

- [Hillier TA, Abbott RD, Barrett EJ. Hyponatremia: evaluating the correction factor for hyperglycemia. Am J Med, 1999.](https://doi.org/10.1016/S0002-9343(99)00055-8)

- [https://pubmed.ncbi.nlm.nih.gov/10225241/](https://pubmed.ncbi.nlm.nih.gov/10225241/)

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

補正ナトリウムは正常：測定された低ナトリウム血症はブドウ糖によるもの（水移動）

| 結果の詳細 | |
| --- | --- |
| 補正ナトリウム（Katz, 1,6） | 138.0 mEq/L |


### 2

補正後でも真の低ナトリウム血症

| 結果の詳細 | |
| --- | --- |
| 補正ナトリウム（Katz, 1,6） | 131.2 mEq/L |


### 3

補正ナトリウム高値：自由水欠乏がある

| 結果の詳細 | |
| --- | --- |
| 補正ナトリウム（Katz, 1,6） | 153.2 mEq/L |

