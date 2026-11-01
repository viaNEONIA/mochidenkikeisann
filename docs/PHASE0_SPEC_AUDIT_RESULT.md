# Phase 0 仕様監査：main照合結果

作成目的: Issue #1 の監査を、実際の `main` の仕様書に照らして更新する。**既存仕様は変更しない。**

## 監査結果

| 監査項目 | mainの確認先 | 結果 |
|---|---|---|
| 基本計算根拠と将来の改訂履歴を区別 | `docs/DECISIONS.md` D007/D008、`docs/CALCULATION_RULES.md`、`docs/SPECIFICATION.md` | 記述整合 |
| 単相100/200V、三相200/400V | `README.md`、`docs/DECISIONS.md` D002 | 記述整合 |
| PDF/CSV・IndexedDB・JSONバックアップ | `docs/SPECIFICATION.md` S08～S10、`docs/DECISIONS.md` D006 | 記述整合 |
| 電圧降下のホーム30A制限と詳細画面 | `docs/SPECIFICATION.md` S03 | 記述整合 |
| 計算結果の保存時点の根拠版 | `docs/SPECIFICATION.md` S08～S10、`docs/CALCULATION_RULES.md` | 記述整合 |
| 未検証の規程値で適合を出さない | `docs/CALCULATION_RULES.md`、`README.md` | 記述整合 |

## 未完了の検証

- 原典の版・利用許諾・数表の転記精度は未検証（Issue #2）。
- 単相3線不平衡、温度・リアクタンスの扱いなど、計算モデルの詳細が未確定（Issue #3）。
- 動力・布設・保護協調の具体的な判定条件が未確定（Issue #4）。
- 電線管とラックの適用表・施工条件が未確定（Issue #5）。
- Android/iOS/PC、オフライン、帳票の実機受入試験は未実施（Issue #6）。

## Issue #1 の完了提案

本書をレビューし、仕様の**記述整合性**に問題がないことを確認できれば Issue #1 をクローズ可能。ただし、これは Phase 0 合格ではない。技術検証は Issue #2～#6 で継続する。

## 注意

本監査は文書間の整合性確認であり、電気計算の正しさ・法令適合性・原典の最新版を保証しない。
