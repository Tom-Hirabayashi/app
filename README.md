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

## Projects記事の追加

```sh
bun run project:new sample-app
```

`src/content/projects/sample-app/sample-app.mdx` が生成されます。記事で使う画像は同じディレクトリに置き、Markdownの相対パスで参照します。

```md
![アプリの画面](./screenshot.png)
```

配布ファイルは `public/files/projects/sample-app/` に置きます。

## 主なディレクトリ

- `src/config/site.toml`: サイト情報、ナビゲーション、テーマなどの設定
- `src/content/about.mdx`: About ページ
- `src/content/blog/`: ブログ記事
- `src/content/projects/<slug>/`: ソフトの紹介・ドキュメントと表示用画像
- `public/files/projects/<slug>/`: Projectsの配布ファイル

## クレジット

Astro と [Navfolio](https://github.com/navfolio/astro-navfolio) を利用しています。
ライセンスについては [LICENSE](./LICENSE) を参照してください。
