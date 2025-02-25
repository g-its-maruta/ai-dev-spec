# cart

## テーブル情報

| 項目                           | 値                                                                                                   |
|:-------------------------------|:-----------------------------------------------------------------------------------------------------|
| システム名                     | AI-APP                                                                                               |
| サブシステム名                 |                                                                                                      |
| スキーマ名                     | data                                                                                                 |
| 物理テーブル名                 | cart                                                                                                 |
| 論理テーブル名                 |                                                                                                      |
| 作成者                         | Y.Maruta                                                                                             |
| 作成日                         | 2024/08/04                                                                                           |
| RDBMS                          | PostgreSQL 10.21 (Debian 10.21-1.pgdg90+1) on aarch64-unknown-linux-gnu, compiled by gcc (Debian 6.3.0-18+deb9u1) 6.3.0 20170516, 64-bit 10.21 |



## カラム情報

| No. | 論理名                         | 物理名                         | データ型                       | Not Null | デフォルト           | 備考                           |
|----:|:-------------------------------|:-------------------------------|:-------------------------------|:---------|:---------------------|:-------------------------------|
|   1 |                                | cartid                         | serial                         | Yes      |                      |                                |
|   2 | 商品ID                         | productid                      | integer                        |          |                      |                                |
|   3 | 数量                           | quantity                       | integer                        | Yes      |                      |                                |



## インデックス情報

| No. | インデックス名                 | カラムリスト                             | ユニーク   | オプション                     | 
|----:|:-------------------------------|:-----------------------------------------|:-----------|:-------------------------------|



## 制約情報

| No. | 制約名                         | 種類                           | 制約定義                       |
|----:|:-------------------------------|:-------------------------------|:-------------------------------|
|   1 | 1559310_1565603_1_not_null     | CHECK                          | productid IS NOT NULL          |
|   2 | 1559310_1565603_2_not_null     | CHECK                          | quantity IS NOT NULL           |
|   3 | 1559310_1565603_3_not_null     | CHECK                          | addedat IS NOT NULL            |



## 外部キー情報

| No. | 外部キー名                     | カラムリスト                             | 参照先                         | 参照先カラムリスト                       | ON DELETE    | ON UPDATE    |
|----:|:-------------------------------|:-----------------------------------------|:-------------------------------|:-----------------------------------------|:-------------|:-------------|
|   1 | cart_productid_fkey            | productid                                | data.products                  | productid                                |              |              |



## 外部キー情報(PK側)

| No. | 外部キー名                     | カラムリスト                             | 参照元                         | 参照元カラムリスト                       | ON DELETE    | ON UPDATE    |
|----:|:-------------------------------|:-----------------------------------------|:-------------------------------|:-----------------------------------------|:-------------|:-------------|


