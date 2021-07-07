# svelte-book-review-app

## 参考サイト

- https://zenn.dev/azukiazusa/books/9dac1257c77f47/viewer/3216ae

## Svelteプロジェクト準備

```shell
npx degit --force sarioglu/svelte-tailwindcss-template .
```

TypeScriptに変換する

```shell
node scripts/setupTypeScript.js
```

## コンポーネントの追加

```shell
mkdir src/components
touch src/components/Header.svelte
```

## ルーティング

```shell
npm install svelte-spa-router
mkdir src/pages/
touch src/pages/SearchBook.svelte
mkdir src/router
touch src/router/index.ts
```
