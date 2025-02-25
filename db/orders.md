# orders

## テーブル情報

| 項目                           | 値                                                                                                   |
|:-------------------------------|:-----------------------------------------------------------------------------------------------------|
| システム名                     | AI-APP                                                                                               |
| サブシステム名                 |                                                                                                      |
| スキーマ名                     | data                                                                                                 |
| 物理テーブル名                 | orders                                                                                               |
| 論理テーブル名                 |                                                                                                      |
| 作成者                         | Y.Maruta                                                                                             |
| 作成日                         | 2024/08/04                                                                                           |
| RDBMS                          | PostgreSQL 10.21 (Debian 10.21-1.pgdg90+1) on aarch64-unknown-linux-gnu, compiled by gcc (Debian 6.3.0-18+deb9u1) 6.3.0 20170516, 64-bit 10.21 |



## カラム情報

| No. | 論理名                         | 物理名                         | データ型                       | Not Null | デフォルト           | 備考                           |
|----:|:-------------------------------|:-------------------------------|:-------------------------------|:---------|:---------------------|:-------------------------------|
|   1 | 注文ID                         | orderid                        | serial                         | Yes (PK) |                      |                                |
|   2 | 注文日時                       | orderdate                      | timestamp(6) without time zone | Yes      |                      |                                |



## インデックス情報

| No. | インデックス名                 | カラムリスト                             | ユニーク   | オプション                     | 
|----:|:-------------------------------|:-----------------------------------------|:-----------|:-------------------------------|
|   1 | orders_pkey                    | orderid                                  | Yes        |                                |



## 制約情報

| No. | 制約名                         | 種類                           | 制約定義                       |
|----:|:-------------------------------|:-------------------------------|:-------------------------------|
|   1 | 1559310_1565613_1_not_null     | CHECK                          | orderid IS NOT NULL            |
|   2 | 1559310_1565613_2_not_null     | CHECK                          | orderdate IS NOT NULL          |
|   3 | orders_pkey                    | PRIMARY KEY                    | orderid                        |



## 外部キー情報

| No. | 外部キー名                     | カラムリスト                             | 参照先                         | 参照先カラムリスト                       | ON DELETE    | ON UPDATE    |
|----:|:-------------------------------|:-----------------------------------------|:-------------------------------|:-----------------------------------------|:-------------|:-------------|



## 外部キー情報(PK側)

| No. | 外部キー名                     | カラムリスト                             | 参照元                         | 参照元カラムリスト                       | ON DELETE    | ON UPDATE    |
|----:|:-------------------------------|:-----------------------------------------|:-------------------------------|:-----------------------------------------|:-------------|:-------------|
|   1 | orderdetails_orderid_fkey      | orderid                                  | data.orderdetails              | orderid                                  |              |              |


