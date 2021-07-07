# svelte-book-review-app

## 参考サイト

- https://zenn.dev/azukiazusa/books/9dac1257c77f47/viewer/3216ae

## 使用技術

- Svelte
- TypeScript
- TailwindCSS
- Google Books API

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

## Repositoryの作成

APIとの通信をRepositoryによって抽象化する  

### httpClientの作成

```shell
npm install axios
mkdir src/repositories
touch src/repositories/httpClient.ts
```

### Book Repositoryの作成

```shell
mkdir src/repositories/book
touch src/repositories/book/types.ts
touch src/repositories/book/BookRepository.ts
touch src/repositories/book/index.ts
```

### Repository Factoryの作成

```shell
touch src/repositories/RepositoryFactory.ts
```

## SearchBarコンポーネントの作成

```shell
touch src/components/SearchBar.svelte
```

## ローディングコンポーネント作成

```shell
touch src/components/Spinner.svelte
```

## BookCardコンポーネント作成

```shell
touch src/components/BookCard.svelte
```
