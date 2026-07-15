# AI開発標準

AIを利用するソフトウェア開発で、品質、安全性、説明可能性、再現性を確保するための共通標準です。特定の製品やリポジトリには依存せず、要件定義から運用・改善までを対象にします。

## 適用方法

1. [基本原則](docs/principles.md)と[開発プロセス](docs/development-process.md)を確認する。
2. 各工程の標準に従って成果物を作成する。
3. `templates/` のひな形と `checklists/` の確認表を利用する。
4. 標準から外れる場合は、理由・影響・代替策・承認者・期限を記録する。

## 標準文書

- [基本原則](docs/principles.md)
- [開発プロセス](docs/development-process.md)
- [要件定義標準](docs/requirements-standard.md)
- [設計標準](docs/design-standard.md)
- [コーディング標準](docs/coding-standard.md)
- [テスト標準](docs/testing-standard.md)
- [セキュリティ標準](docs/security-standard.md)
- [AI利用標準](docs/ai-usage-standard.md)
- [レビュー標準](docs/review-standard.md)
- [リリース標準](docs/release-standard.md)

## 適用レベル

文中の「必須」は原則として省略できません。「推奨」は、採用しない理由を説明できる状態にします。プロジェクト固有ルールが本標準より厳しい場合は、厳しい方を適用します。

## 変更方法

標準の変更は Pull Request で行い、目的、影響範囲、移行方法を記載します。破壊的変更には適用開始日と移行期間を設けます。

## ライセンス

現時点では利用許諾条件を定めていません。詳細は [LICENSE](LICENSE) を参照してください。
