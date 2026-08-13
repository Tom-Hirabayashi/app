# ひらともWEB

国語の授業や校務に役立つフリーソフトを紹介するサイトです。

サイト: <https://tom-hirabayashi.github.io/app/>

## 開発

必要な環境:

- Node.js 22.12 以上
- Bun
- Python 3、FontTools、Brotli（本番ビルド時）

```sh
bun install
bun run dev
```

本番ビルド:

```sh
bun run build
```

## 主なディレクトリ

- `src/config/site.toml`: サイト情報、ナビゲーション、テーマなどの設定
- `src/content/about.mdx`: About ページ
- `src/content/blog/`: ブログ記事
- `src/content/projects/`: ソフトの紹介・ドキュメント
- `public/files/`: 配布ファイル

## クレジット

Astro と [Navfolio](https://github.com/navfolio/astro-navfolio) を利用しています。
ライセンスについては [LICENSE](./LICENSE) を参照してください。
