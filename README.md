# package.json

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
pnpm install
```

### Compile and Hot-Reload for Development

```sh
pnpm dev
```

### Compile and Minify for Production

```sh
pnpm build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
pnpm test:unit
```

### Run End-to-End Tests with [Cypress](https://www.cypress.io/)

```sh
pnpm test:e2e:dev
```

This runs the end-to-end tests against the Vite development server.
It is much faster than the production build.

But it's still recommended to test the production build with `test:e2e` before deploying (e.g. in CI environments):

```sh
pnpm build
pnpm test:e2e
```

### Lint with [ESLint](https://eslint.org/)

```sh
pnpm lint
```

## 思路

自动引入 module 模块。需要自己手动导入
antd 引入最新版本
pug 语法，写法更轻便
nocss 原子css 简便写法
引入的模块 自定义声明 .ts 文件类型(js ts两个版本说明)
pnpm 包使用

权限系统
项目内外联 组件或自定义方法

整理编写文章

antd 封装组件说明
grid 布局，表单查询多个，默认展示一行，点击更多展开更多

### Ant Design Vue

[Ant Design Vue传送阵](https://www.antdv.com/components/overview)

### PUG 语法安装

    pnpm i pug pug-html-loader --save-dev

vue

```html
<template lang="pug"> div h1 Hello PUG! span Hello Span Tag </template>
```

若 Vite 中引用

    pnpm add vite-plugin-pug --save-dev

`vite.config.js` 配置

```js
import pug from 'vite-plugin-pug'
export default defineConfig({
  plugins: [
    pug({
      /** 插件选项 */
    })
  ]
})
```
