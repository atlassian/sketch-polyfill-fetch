# sketch-polyfill-fetch-babel-safe

**This is a (hopefully temporary) fork of `sketch-polyfill-fetch` that uses `cocoascript-class-babel-safe`, to allow safe transpilation to ES5.**

A [fetch](https://developer.mozilla.org/en/docs/Web/API/Fetch_API) polyfill for sketch inspired by [unfetch](https://github.com/developit/unfetch). It is automatically included (when needed) when using [skpm](https://github.com/skpm/skpm).

## Installation

```bash
npm i -S sketch-polyfill-fetch
```

## Usage

```js
import fetch from 'sketch-polyfill-fetch'

fetch("https://google.com")
  .then(response => response.text())
  .then(text => console.log(text))
  .catch(e => console.error(e))
```
