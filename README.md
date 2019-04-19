# StealJS plugin for Literate JavaScript

## Installation

```console
$ npm install --save steal-lavascript
```

## Use

To use this plugin load a `js.md` file with the bang syntax.

```js
const otherFile = require('./otherFile.js.md!lavascript')
```

```js
import otherFile from './otherFile.js.md!lavascript'
```

If you wanted to associate all `.js.md` files with the `steal-lavascript` plugin, you could specify it as a handler using the `ext` property in your `steal` configuration.

```js
"steal": {
  "ext": {
    "js.md": "lavascript"
  }
}
```

With the above configuration, you can import a `lavascript` file as you would any other file.

```js
const otherFile = require('./otherFile.js.md')
```

```js
import otherFile from './otherFile.js.md'
```