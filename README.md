# boatrace2
競艇予想を行うためのプロジェクト. 下記の機能があります。
1. データベース作成. これまでのレース結果をpandas dfに格納
2. データ解析

リポジトリをクローンして使用してください。

`git clone https://github.com/griCe14807/boatrace2.git`

### 1. データベースの作成
1_クロール、スクレイプ、データ格納.ipynb
- ボートレースのデータを日付ごとにpickleファイルでdata/crawledDataフォルダに保存

2_データ前処理（共通部分).ipynb
-  crawledDataフォルダに格納されたファイルを一つのdfにまとめ、data/arrangedDataフォルダに保存
- この際、データ分析に使えるよう、各列のデータタイプや値などを整理・調整

### 2. データ解析
- 3.1 以降の数字がついたipythonファイルは全てデータ解析を行ったファイル
- それぞれ、targetの設定や特徴量の設定などを変えて実行している。番号は時系列順


## boatraceからの改善点
Databaseを、
目的に応じた統計量を自分で算出し、特徴量として使用しやすくする。
できるようにするため、下記の通り変更した。形のXX...