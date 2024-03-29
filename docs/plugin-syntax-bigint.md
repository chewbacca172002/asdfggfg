---
id: babel-plugin-syntax-bigint
title: "@babel/plugin-syntax-bigint"
sidebar_label: syntax-bigint
---

:::info
This plugin is included in `@babel/preset-env`, in [ES2020](https://github.com/tc39/proposals/blob/master/finished-proposals.md)
:::

:::note
#### Syntax only

This plugin only enables parsing of this feature. Babel doesn't support transforming BigInts. One recommendation is to use the JSBI library and eventually run `babel-plugin-transform-jsbi-to-bigint` to codemod it to BigInt in the future.
:::

## Installation

```shell npm2yarn
npm install --save-dev @babel/plugin-syntax-bigint
```

## Usage

### With a configuration file (Recommended)

```json title="babel.config.json"
{
  "plugins": ["@babel/plugin-syntax-bigint"]
}
```

### Via CLI

```sh title="Shell"
babel --plugins @babel/plugin-syntax-bigint script.js
```

### Via Node API

```js title="JavaScript"
require("@babel/core").transformSync("code", {
  plugins: ["@babel/plugin-syntax-bigint"],
});
```

## References

- [proposal-bigint](https://github.com/tc39/proposal-bigint)
- [BigInt from v8.dev](https://v8.dev/features/bigint#polyfilling-transpiling)
- [babel-plugin-transform-jsbi-to-bigint](https://github.com/GoogleChromeLabs/babel-plugin-transform-jsbi-to-bigint)
