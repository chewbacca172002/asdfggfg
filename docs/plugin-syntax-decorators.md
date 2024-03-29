---
id: babel-plugin-syntax-decorators
title: "@babel/plugin-syntax-decorators"
sidebar_label: syntax-decorators
---

:::note
#### Syntax only

It's unlikely you want to use this plugin directly as it only enables Babel to parse this syntax. Instead, use [plugin-proposal-decorators](plugin-proposal-decorators.md) to _both_ parse and transform this syntax.
:::

## Installation

```shell npm2yarn
npm install --save-dev @babel/plugin-syntax-decorators
```

## Usage

### With a configuration file (Recommended)

```json title="babel.config.json"
{
  "plugins": ["@babel/plugin-syntax-decorators"]
}
```

### Via CLI

```sh title="Shell"
babel --plugins @babel/plugin-syntax-decorators script.js
```

### Via Node API

```js title="JavaScript"
require("@babel/core").transformSync("code", {
  plugins: ["@babel/plugin-syntax-decorators"]
});
```

## Options

This plugin accepts the same options as [`@babel/plugin-proposal-decorators`](plugin-proposal-decorators.md).

:::tip
You can read more about configuring plugin options [here](https://babeljs.io/docs/en/plugins#plugin-options)
:::
