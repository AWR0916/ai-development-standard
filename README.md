# AI開発標準

AIを利用するソフトウェア開発で、品質、安全性、説明可能性、再現性を確保するための共通標準です。特定の製品やリポジトリには依存せず、要件定義から運用・改善までを対象にします。

## 現在のバージョン

現在の標準バージョンは [VERSION](VERSION) に記載します。変更内容は [CHANGELOG](CHANGELOG.md)、互換性と更新規則は[バージョニング方針](docs/versioning-policy.md)を参照してください。

各プロジェクトは、既定ブランチではなく採用したバージョンタグを固定参照します。

## 適用方法

1. [基本原則](docs/principles.md)と[開発プロセス](docs/development-process.md)を確認する。
2. [導入ガイド](ADOPTION.md)に従い、対象リポジトリへ適用バージョンと[適用プロファイル](docs/profiles.md)を記録する。
3. 各工程の標準に従って成果物を作成する。
4. `templates/` のひな形と `checklists/` の確認表を利用する。
5. 標準から外れる場合は、[導入ガイドの例外](ADOPTION.md#例外)に従い、対象規則、理由、影響、代替策と確認方法、承認者、有効期限、再評価日を記録する。

## 標準文書

- [基本原則](docs/principles.md)
- [適用プロファイル](docs/profiles.md)
- [開発プロセス](docs/development-process.md)
- [要件定義標準](docs/requirements-standard.md)
- [設計標準](docs/design-standard.md)
- [コーディング標準](docs/coding-standard.md)
- [テスト標準](docs/testing-standard.md)
- [セキュリティ標準](docs/security-standard.md)
- [AI利用標準](docs/ai-usage-standard.md)
- [レビュー標準](docs/review-standard.md)
- [リスク区分と役割](docs/risk-and-roles.md)
- [リリース標準](docs/release-standard.md)
- [運用標準](docs/operations-standard.md)
- [バージョニング方針](docs/versioning-policy.md)
- [用語集](docs/glossary.md)

## 導入資材

- [導入ガイド](ADOPTION.md)
- [AGENTS.md導入テンプレート](templates/adoption/AGENTS.md)
- [導入用Pull Requestテンプレート](templates/adoption/pull_request_template.md)
- [適合確認チェックリスト](checklists/adoption-checklist.md)
- [再利用可能な文書検査](.github/workflows/reusable-documentation-check.yml)

## テンプレートとチェックリスト

| 工程 | テンプレート | チェックリスト |
|---|---|---|
| 要件定義 | [要件定義](templates/requirements-template.md)、[データ分類とAI利用](templates/data-classification-template.md) | — |
| 設計 | [設計](templates/design-template.md)、[脅威分析](templates/threat-model-template.md)、[ADR](templates/adr-template.md) | [設計レビュー](checklists/design-review-checklist.md)、[セキュリティ](checklists/security-checklist.md) |
| 実装・レビュー | [追跡表](templates/traceability-matrix-template.md) | [Pull Request](checklists/pull-request-checklist.md)、[AI利用](checklists/ai-usage-checklist.md) |
| 検証 | [テスト計画](templates/test-plan-template.md) | [テスト](checklists/test-checklist.md) |
| リリース | — | [リリース](checklists/release-checklist.md) |
| 導入・例外 | [例外](templates/exception-template.md) | [適合確認](checklists/adoption-checklist.md) |

## 適用レベル

検証可能な規則には、`SEC-01（必須）` のように規則IDと適用レベルを付けます。規則IDの形式と接頭辞は[バージョニング方針](docs/versioning-policy.md#規則id)に定めます。文書に記載した適用レベルは「標準」プロファイルでのレベルです。試作と高保証での違いは[適用プロファイル](docs/profiles.md)に定めます。基本原則は判断の拠り所であり、規則IDを付けません。

「必須」は原則として省略できません。「推奨」は、採用しない理由を説明できる状態にします。プロジェクト固有ルールが本標準より厳しい場合は、厳しい方を適用します。例外やチェックリストでは、対象の規則を規則IDで示します。

## 変更方法

標準の変更は Pull Request で行い、目的、影響範囲、移行方法を記載します。破壊的変更には適用開始日と移行期間を設けます。

## ライセンス

文書、テンプレート、チェックリストは [クリエイティブ・コモンズ 表示 4.0 国際（CC BY 4.0）](LICENSE) で提供します。出典を表示すれば、組織内での利用、改変、再配布ができます。

ワークフローと設定ファイルは [MIT License](LICENSE-CODE) で提供します。
