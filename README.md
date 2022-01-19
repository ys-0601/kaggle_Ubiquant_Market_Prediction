![comp](./images/Ubiquant_Market_Prediction.png)
# kaggle_Ubiquant_Market_Prediction
Kaggle-Ubiquant Market Prediction コンペのリポジトリ

- result
  - public: 0.000
  - private: 0.000
  - rank: 0000/9999

    <img src='./images/ranking.png' width='500'>



- directory tree
```
nishika_prediction_of_second-hand_apartment_2022winter
├── README.md
├── data         <---- kaggle提供データ
├── images       <---- readme用画像
├── program      <---- jupyter lab用ノートブック
      ├──std     <---- post時のノートブック
      ├──edit    <---- 作業用ノートブック
```

## Pipeline
- 実行例
  ```bash
  #python3 pipeline.py --globals.balanced=1 --globals.comment=test
  ```

- 結果の表示例
  ```bash
  #python3 show_result.py -d 0
  ```



## Info
- [issue board](https://github.com/ys-0601/kaggle_Ubiquant_Market_Prediction/projects/1)   <---- これ大事だよ
- ref:


## Timeline

<img src='./images/timeline.png' width='1000'>

## External Dataset
|Name|Detail|Ref|
|---|---|---|
|---|---|---|

## Modularized file
|Name|Detail|In|Out|
|---|---|---|---|
|---|---|---|---|

## Features
|Name|structure|type|Detail|
|---|---|---|---|
|---|---|---|---|
|---|---|---|---|
|---|---|---|---|
|---|---|---|---|
|---|---|---|---|



## Paper/Reference
|No.|Status|Name|Detail|Date|Url|
|---|---|---|---|---|---|
|00|<font color='orange'>Todo</font>|Kaggle日記という戦い方|kaggle日記参照元。|2021/06|[url](https://zenn.dev/fkubota/articles/3d8afb0e919b555ef068)|
|01|<font color='gray'>Doint</font>|---|---|---|[url]()|
|02|<font color='gray'>Done</font>|---|---|---|[url]()|
|03|<font color='gray'>Doint</font>|---|---|---|[url]()|
|04|<font color='gray'>Done</font>|---|---|---|[url]()|
|05|<font color='gray'>Done</font>|---|---|---|[url]()|
|06|<font color='gray'>Doint</font>|---|---|---|[url]()|
|07|<font color='gray'>Done</font>|---|---|---|[url]()|
|08|<font color='gray'>Done</font>|---|---|---|[url]()|
|09|<font color='gray'>Done</font>|---|---|---|[url]()|
|10|<font color='gray'>Done</font>|---|---|---|[url]()|
|11|<font color='gray'>Done</font>|---|---|---|[url]()|
|12|<font color='gray'>Done</font>|---|---|---|[url]()|
|13|<font color='gray'>Done</font>|---|---|---|[url]()|
|14|<font color='gray'>Done</font>|---|---|---|[url]()|
|15|<font color='gray'>Done</font>|---|---|---|[url]()|

## Memo
- term
  - nb: ノートブック
  - ----


## Basics
**背景と目的**

Ubiquant Market Prediction-ユビキタス・マーケット・プレディクション
将来の市場データに対して予測を行う

投資戦略にかかわらず、金融市場には変動がつきものです。この変動にもかかわらず、プロの投資家は全体的なリターンを推定しようとします。リスクとリターンは投資の種類やその他の要因によって異なり、安定性とボラティリティに影響を及ぼします。リターンの予測を試みるために、金融市場の取引にはコンピュータを使ったアルゴリズムやモデルが多く存在します。しかし、新しい手法やアプローチにより、データサイエンスは定量的研究者の投資リターンの予測能力を向上させることができる。



ユビキント・インベストメント（北京）有限公司は、中国を拠点とする国内有数のクオンツ・ヘッジファンドです。2012年に設立され、数学とコンピュータサイエンスの国際的な才能と最先端技術を駆使して、金融市場のクオンツ投資を推進しています。ユビキタントは、投資家のために長期的に安定したリターンを創出することに取り組んでいます。

このコンペティションでは、投資の収益率を予測するモデルを構築していただきます。過去の価格を用いてアルゴリズムをトレーニングし、テストしてください。優秀な作品は、この実世界のデータサイエンス問題を可能な限り正確に解決します。

成功すれば、定量的研究者のリターン予測能力を向上させることができます。これにより、あらゆる規模の投資家がより良い意思決定を行えるようになります。また、自分が金融データセットに長けていることがわかり、多くの業界で新しいチャンスが広がるかもしれません。


**data(deepL)**   
ファイル内容
このデータセットには、何千もの投資案件の実際の履歴データから得られた特徴が含まれています。あなたの課題は、取引の意思決定に関連する難解な指標の値を予測することです。

これは、時系列APIに依存するコードコンペティションで、モデルが時間を遡ることがないようにするものです。APIを使用するには、評価ページの指示に従います。ノートブックを提出すると、そのノートブックは未知のテストで再実行されます。これは予測コンペティションでもあり、最終的なプライベートリーダーボードはトレーニング期間終了後に収集されたデータを使って決定されるため、パブリックリーダーボードとプライベートリーダーボードの重なりはゼロになります。

ファイル名
train.csv

row_id - その行に一意な識別子。
time_id - データが収集された時刻のIDコード。time IDは順番に並んでいますが、time ID間の実時間は一定ではなく、トレーニングセットよりも最終的なプライベートテストセットの方が短くなる可能性が高いです。
investment_id - 投資のIDコード。すべての投資先がすべての時間IDにデータを持つわけではない。
target - ターゲット。
[f_0:f_299] - マーケットデータから生成された匿名化された特徴量。
example_test.csv - 投入時にAPIがどのような形とフォーマットのデータをあなたのノートブックに配信するかを示すために提供されるランダムなデータです。

example_sample_submission.csv - 一般にアクセス可能な API のコピーが正しいデータの形と形式を提供するように提供される、投稿ファイルの例です。

ubiquant/ - テストセットを提供する画像配信API。テストセットのサンプルをオフラインでエラーなく実行するには、Python 3.7 と Linux 環境が必要な場合があります。

時系列APIの詳細 - このAPIはバッチごとにデータを提供し、バッチごとに1つのtime_idを持つ。

テストセットには約100万行が含まれる予定である。

APIは初期化後、約0.25GBのメモリを必要とする。初期化ステップ(env.iter_test())で必要なメモリは、それよりもかなり多いので、この呼び出しを行うまでモデルをロードしないことをお勧めします。

また、APIの実行時間は、データのロードと配信に15分未満を予定しています。



### train.csv colomn infomaiton
notebook: eda01.ipynb
example: https://panasonic-cns.udemy.com/course/python-data/learn/lecture/25769636?start=0#content

|name|Explanation|Detail|
|----|----|----|----|
|----|----|----|----|
|----|----|----|----|
|----|----|----|----|



## Log
### 20210119
- join!!
- 参戦の環境構築(git/gitHub)・twitter・Readme・データのダウンロード


