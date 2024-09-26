# 遊ぶこと
OSSのBIツール「metabase」を使ってみる。

以下をやってみる
https://zenn.dev/sikkim/articles/6866b32919372d

# 実行手順
1. 開発コンテナを起動
2. JARを実行
   ```sh
   java -jar metabase.jar
   ```
3. `http://localhost:3000/setup`にアクセス

# 環境構築
`環境構築.md`を参照。

# ディレクトリ構造
`plugins/`および`.git`以下は省略。

以下は`.gitignore`で定義。  
ファイルサイズが大きいもの、引用元があるファイル、metabase実行時の生成ファイルを記載している。
- plugins
- metabase.db.mv.db
- metabase.db.trace.db
- metabase.jar
- app/db/files
- app/db/load.sql

```sh
$ tree
.
├── .devcontainer
│   └── devcontainer.json
├── .git
├── .gitignore
├── README.md
├── app
│   ├── build
│   │   └── compose.yaml
│   └── db
│       ├── files
│       │   ├── access_log.csv
│       │   ├── access_log.ct
│       │   ├── customers.csv
│       │   ├── customers.ct
│       │   ├── items.csv
│       │   ├── items.ct
│       │   ├── order_details.csv
│       │   ├── order_details.ct
│       │   ├── orders.csv
│       │   ├── orders.ct
│       │   ├── shops.csv
│       │   ├── shops.ct
│       │   ├── web_pages.csv
│       │   └── web_pages.ct
│       └── load.sql
├── java-install.sh
├── metabase.db.mv.db
├── metabase.db.trace.db
├── metabase.jar
├── plugins
├── postgres.md
└── 環境構築.md
```
