# 根拠レコード・スキーマ案 v0.1

以下は設計提案であり、実データ登録や規程値の確定ではない。

```json
{
  "sourceId": "SRC-EXAMPLE",
  "category": "manufacturer-catalog",
  "title": "未登録",
  "publisher": null,
  "edition": null,
  "publishedOn": null,
  "sourceUrl": null,
  "sourceLocation": null,
  "sectionOrTable": null,
  "applicability": {
    "productFamily": null,
    "installationMethod": null,
    "ambientTemperatureC": null,
    "grouping": null,
    "notes": null
  },
  "usageRights": {
    "reviewed": false,
    "redistributionAllowed": null,
    "notes": null
  },
  "status": "unverified",
  "verifiedBy": null,
  "verifiedAt": null,
  "reviewEvidence": [],
  "supersedes": null
}
```

## 運用規則
- sourceId は一意。改訂版は別IDとする。
- 未検証の数値を仮の「代表値」として登録しない。
- 外部原典を参照できても再配布権限がなければ、数表をリポジトリに複製しない。
- 利用可能なマスター値は、個別に sourceId・条件・単位・検証日時を持つ。
- 保存済み計算には sourceId、版、実際の代入値を記録する。
