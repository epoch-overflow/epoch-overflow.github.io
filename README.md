# epoch-overflow.github.io

2038年問題をはじめとする、時刻表現の桁あふれ問題についての日本語情報サイトのソースです。

公開URL: <https://epoch-overflow.github.io/>

## ローカルでの確認

```sh
pip install zensical
zensical serve      # http://localhost:8000/ でプレビュー
zensical build      # site/ に静的ファイルを生成
```

## 構成

```text
.
├── zensical.toml              # サイト設定（ナビゲーションもここで定義）
├── docs/                      # 本文（Markdown）
│   ├── index.md
│   ├── y2038/                 # 2038年問題
│   ├── overflow/              # 時刻の桁あふれ問題全般（GPS rollover など）
│   ├── references.md
│   └── about.md
└── .github/workflows/docs.yml # main への push で GitHub Pages にデプロイ
```

ページを追加したら、`zensical.toml` の `nav` にも追記してください。

## ライセンス

- 本文（`docs/` 以下の文章・図）: [CC BY 4.0](LICENSE)
- コード（設定ファイル、ワークフロー、スクリプト等）: [BSD-2-Clause](LICENSE-CODE)

## アイコン

ロゴとアイコンは [Lucide](https://lucide.dev) の [`rotate-ccw-clock`](https://lucide.dev/icons/rotate-ccw-clock) アイコンをもとに配色を変えたものです（ISC License, Copyright (c) Lucide Icons and Contributors。全文は [LICENSE-LUCIDE](LICENSE-LUCIDE)）。

- サイト用（`docs/assets/logo.svg`）：背景は透明、矢印 `#b91c1c`、針 `#6b7280`
- サイト用の大きいサイズ（`branding/logo-512.svg` / `logo-512.png`）：上と同じデザインで 512×512、背景透明
- GitHub 用（`branding/avatar.png`）：背景 `#b91c1c`、アイコン白
