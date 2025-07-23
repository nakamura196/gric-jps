# Japan Search SPARQL API

Japan SearchのSPARQLエンドポイントを使用したgrlc APIです。

## 利用可能なエンドポイント

- `/search_with_enum` - 文化財タイプ別検索（選択式）
- `/list_types` - 利用可能な文化財タイプ一覧

## 使用方法

```bash
# 文化財タイプ別検索（デフォルト：絵画）
curl "http://grlc.io/api-git/nakamura196/grlc-jps/search_with_enum"

# 特定のタイプを指定して検索
curl "http://grlc.io/api-git/nakamura196/grlc-jps/search_with_enum?type=https://jpsearch.go.jp/term/type/古書・古文書"

# 利用可能なタイプ一覧を取得
curl "http://grlc.io/api-git/nakamura196/grlc-jps/list_types"
```

### 利用可能な文化財タイプ

- 絵画: `https://jpsearch.go.jp/term/type/絵画`
- 古書・古文書: `https://jpsearch.go.jp/term/type/古書・古文書`
- 写真: `https://jpsearch.go.jp/term/type/写真`
- 彫刻: `https://jpsearch.go.jp/term/type/彫刻`
- 工芸: `https://jpsearch.go.jp/term/type/工芸`
- 建造物: `https://jpsearch.go.jp/term/type/建造物`
- 史跡: `https://jpsearch.go.jp/term/type/史跡`

## データソース

このAPIは[ジャパンサーチ](https://jpsearch.go.jp/)のSPARQLエンドポイントを使用しています。

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE)ファイルをご覧ください。

## 注意事項

- ジャパンサーチの利用規約に従ってご利用ください
- 大量のリクエストは避けてください
- データの著作権は各提供機関に帰属します
