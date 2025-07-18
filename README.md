# tpcds

## SQLクエリ最適化ワークショップ

**ノートブック**: `SQLTuningWorkshop ver 1.1.dbc`

本ワークショップでは、クエリプロファイルを使用したクエリの実行状況の分析と最適化手法をウォークスルーしながら、実践的なServerless SQLのパフォーマンスチューニング方法を学びます。

### 参考資料

- **公式ドキュメント**: [Query profile | Databricks on AWS](https://docs.databricks.com/aws/ja/sql/user/queries/query-profile)
- **参考記事**: [Qiita - Databricks SQL クエリプロファイルを使ったパフォーマンスチューニング](https://qiita.com/Mitsuhiro_itagaki/items/8f8334797e11a4aafd53)

## 前提条件

### データセット準備
- 事前にTPC-DSのデータセットが作成されていること
- **ノートブック**: `TPC-datagen-notebook_UC.dbc`
- TPC-DS data generator to run as a job ノートブックでスケールファクターを1000(1000GB)で実行し、テスト用データを事前に作成しておいてください

### 権限要件
- ユーザはServerless SQL(L)サイズに対するCan Monitor権限以上を付与されていること（SparkUIを使用するため）

## ファイル構成

- `SQLTuningWorkshop ver 1.1.dbc` - SQLクエリ最適化ワークショップ用ノートブック
- `TPC-datagen-notebook_UC.dbc` - TPC-DSデータ生成用ノートブック
- `TPCDS_Queries_notebook.zip` - TPC-DSクエリ集