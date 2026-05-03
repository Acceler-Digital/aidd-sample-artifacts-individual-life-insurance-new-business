# AI駆動開発 成果物サンプル - 生命保険 新契約システム

[AI駆動開発テンプレート](https://github.com/Acceler-Digital/aidd-artifacts-template)（以下、AIDDテンプレート）を使って実プロジェクトを進めた場合に、どのような成果物体系が生まれるのかを具体的に示すサンプルリポジトリです。

実在の企業ではなく、架空の生命保険会社「Sample生命保険株式会社」における 個人保険（終身保険・定期保険・医療保険・がん保険 等）の新契約手続きWebという題材で、プロジェクト管理に関する一連の成果物を配置しています。

## 何が置いてあるか

成果物は [docs/](docs/) 配下に、AIDDテンプレートで定義されたフェーズ区分で収録しています。

| フェーズ | ディレクトリ | 主な成果物 |
|---|---|---|
| **D0** プロジェクト管理 | [docs/D0.project-management/](docs/D0.project-management/) | プロジェクトインデックス、成果物フロー |

フェーズ間の依存関係や成果物の生成順については [docs/D0.project-management/artifact-flow.md](docs/D0.project-management/artifact-flow.md) を参照してください。

## ドキュメントサイトをローカルで立ち上げる

[docs/](docs/) 配下のMarkdownは [Docusaurus 3](https://docusaurus.io/) でWikiサイトとしてプレビューできます。サイドバー構成は [sidebars.ts](sidebars.ts) を参照ください。

```bash
# 依存関係インストール
pnpm install

# 開発サーバー起動（ホットリロード付き）
pnpm start
# → http://localhost:3000 で閲覧

# 本番ビルド
pnpm build

# ビルド後のプレビュー
pnpm serve

# オフライン閲覧用ビルド（hash router・検索インデックス同梱）
pnpm build:offline
```

### 前提条件

- Node.js 18 以上
- pnpm 9 以上

## リポジトリ構成

```
.
├── docs/                        # 成果物本体（本サンプルでは D0 のみ収録）
│   └── D0.project-management/
├── scripts/                     # オフラインビルド用スクリプト
├── sidebars.ts                  # Docusaurus サイドバー定義
├── docusaurus.config.ts         # Docusaurus 設定
└── package.json
```

## 関連リポジトリ

- [aidd-artifacts-template](https://github.com/Acceler-Digital/aidd-artifacts-template) — 本サンプルの元となるAI駆動開発テンプレート本体

## ライセンス

本リポジトリに含まれるドキュメント・図・設定ファイルは [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) の下で提供されます。全文は同梱の [LICENSE](LICENSE) を参照してください。
