# 遊ぶこと
OSSのBIツール「metabase」を使ってみる。

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
```sh
$ tree
.
├── .devcontainer
│   └── devcontainer.json
├── .git
├── .gitignore
├── README.md
├── java-install.sh
├── metabase.db.mv.db
├── metabase.db.trace.db
├── metabase.jar
├── plugins
└── 環境構築.md
```

