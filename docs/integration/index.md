---
canonical_language: ja-JP
publication_batch: 2026-10-19
translation_status: canonical-editorial-projection
---

# SphereOS・Foldとの接続

Quantarilの統合面では、nodeの自律性と、必要な意味・因果・権限・receiptの交換条件を扱います。

| 面 | 確認する責務 |
|---|---|
| World／node | local state、local clock、owner authority |
| SphereOS | World管理・隔離・資源・復旧の上流契約 |
| Fold | 意味・protocol・Identity／Authority等の接続条件 |
| IBD等 | 保存・取得・同期のcomponent契約 |
| 本site | 統合の説明、sourceと検証状態の索引 |

同じ構成図に置くことは実装依存や権限の継承ではありません。接続にはrevision、capability、入出力、失敗・停止・復旧条件を明示します。

最初の実験として、同じsource状態を持つ二nodeを想定し、接続・切断・再接続ごとに、保持した状態・交換した情報・失われた文脈を比較できます。実装で試した場合だけcommitと結果を追加します。机上例からP2P runtime完成を主張しません。

[English reference manuscript](https://github.com/HIPSTAR-IScompany/quantaril/blob/main/i18n/en/docusaurus-plugin-content-docs/current/integration/index.md)。日本語を正本とする編集解説です。原典の契約を変更しません。

著者: 齋藤みつるSaitooMituru-Fusamofu-ふさもふ。原典の個別creditは各出典を参照。文書: CC BY 4.0。

## 出典

- [docs/theory/quantaril-cloud.ja.md](https://github.com/saitoomituru/ZeroRoomLab-manifest/blob/139cc619fcdd62f254074e655ad3fb04e190322d/docs/theory/quantaril-cloud.ja.md)
- [docs/theory/sphereos-atlantis-versioning-and-bootstrap.ja.md](https://github.com/saitoomituru/ZeroRoomLab-manifest/blob/139cc619fcdd62f254074e655ad3fb04e190322d/docs/theory/sphereos-atlantis-versioning-and-bootstrap.ja.md)
