# AI開発標準

AIを利用するソフトウェア開発で、品質、安全性、説明可能性、再現性を確保するための共通標準です。特定の製品やリポジトリには依存せず、要件定義から運用・改善までを対象にします。

## 現在のバージョン

現在の標準バージョンは [VERSION](VERSION) に記載します。変更内容は [CHANGELOG](CHANGELOG.md)、互換性と更新規則は[バージョニング方針](docs/versioning-policy.md)を参照してください。

各プロジェクトは、既定ブランチではなく採用したバージョンタグを固定参照します。

## 適用方法

1. [基本原則](docs/principles.md)と[開発プロセス](docs/development-process.md)を確認する。
2. [導入ガイド](ADOPTION.md)に従い、対象リポジトリへ適用バージョンを記録する。
3. 各工程の標準に従って成果物を作成する。
4. `templates/` のひな形と `checklists/` の確認表を利用する。
5. 標準から外れる場合は、[導入ガイドの例外](ADOPTION.md#例外)に従い、対象規則、理由、影響、代替策と確認方法、承認者、有効期限、再評価日を記録する。

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
- [バージョニング方針](docs/versioning-policy.md)

## 導入資材

- [導入ガイド](ADOPTION.md)
- [AGENTS.md導入テンプレート](templates/adoption/AGENTS.md)
- [適合確認チェックリスト](checklists/adoption-checklist.md)
- [再利用可能な文書検査](.github/workflows/reusable-documentation-check.yml)

## 適用レベル

文中の「必須」は原則として省略できません。「推奨」は、採用しない理由を説明できる状態にします。プロジェクト固有ルールが本標準より厳しい場合は、厳しい方を適用します。

## 変更方法

標準の変更は Pull Request で行い、目的、影響範囲、移行方法を記載します。破壊的変更には適用開始日と移行期間を設けます。

## ライセンス

現時点では利用許諾条件を定めていません。詳細は [LICENSE](LICENSE) を参照してください。
