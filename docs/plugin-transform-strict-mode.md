---
id: babel-plugin-transform-strict-mode
title: babel-plugin-transform-strict-mode
sidebar_label: transform-strict-mode
---

This plugin may be enabled via `@babel/plugin-transform-modules-commonjs`.
If you wish to disable it you can either turn `strict` off or pass
`strictMode: false` as an option to the commonjs transform.

## Example

**In**

```javascript
foo();
```

**Out**

```javascript
"use strict";

foo();
```

## Installation

```sh
npm install --save-dev @babel/plugin-transform-strict-mode
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**


```json
{
  "plugins": ["@babel/plugin-transform-strict-mode"]
}
```


### Via CLI

```sh
babel --plugins @babel/plugin-transform-strict-mode script.js
```

### Via Node API

```javascript
require("@babel/core").transform("code", {
  plugins: ["@babel/plugin-transform-strict-mode"]
});
```

