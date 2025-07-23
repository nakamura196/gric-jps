# Japan Search SPARQL API

Japan SearchのSPARQLエンドポイントを使用したgrlc APIです。

## 利用可能なエンドポイント

- `/ancient_books` - 古書・古文書の検索
- `/test_simple` - 基本的なテストクエリ

## 使用方法

```bash
# 古書・古文書を検索
curl "http://grlc.io/api-git/nakamura196/gric-jps/ancient_books"

# 基本テスト
curl "http://grlc.io/api-git/nakamura196/gric-jps/test_simple"
```

## データソース

このAPIは[ジャパンサーチ](https://jpsearch.go.jp/)のSPARQLエンドポイントを使用しています。

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE)ファイルをご覧ください。

## 注意事項

- ジャパンサーチの利用規約に従ってご利用ください
- 大量のリクエストは避けてください
- データの著作権は各提供機関に帰属します
