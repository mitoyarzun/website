---
id: babel-plugin-proposal-throw-expressions
title: babel-plugin-proposal-throw-expressions
sidebar_label: proposal-throw-expressions
---

## Example

```js
function test(param = throw new Error('required!')) {
  const test = param === true || throw new Error('Falsey!');
}
```

## Installation

```sh
npm install --save-dev @babel/plugin-proposal-throw-expressions
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["@babel/plugin-proposal-throw-expressions"]
}
```

### Via CLI

```sh
babel --plugins @babel/plugin-proposal-throw-expressions script.js
```

### Via Node API

```javascript
require("@babel/core").transform("code", {
  plugins: ["@babel/plugin-proposal-throw-expressions"]
});
```

## References

* [Proposal: ECMAScript throw expressions](https://github.com/tc39/proposal-throw-expressions)

