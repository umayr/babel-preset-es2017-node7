# babel-preset-es2017-node7 [![](https://img.shields.io/npm/v/babel-preset-es2017-node7.svg)](https://npmjs.org/package/babel-preset-es2017-node7)

> Babel preset to make node@7 ES2017 compatible.

Node@7 has great [ES2017 support](https://nodejs.org/en/docs/es6/), and this module just adds missing features:

- modules ([transform-es2015-modules-commonjs](http://babeljs.io/docs/plugins/transform-es2015-modules-commonjs))
- class properties ([transform-class-properties](http://babeljs.io/docs/plugins/transform-class-properties))
- object rest spread ([syntax-object-rest-spread](http://babeljs.io/docs/plugins/syntax-object-rest-spread))
- trailing function commas ([syntax-trailing-function-commas](http://babeljs.io/docs/plugins/syntax-trailing-function-commas))
- async to generator ([transform-async-to-generator](https://babeljs.io/docs/plugins/transform-async-to-generator/))

## Install

```js
$ npm install --save-dev babel-preset-es2017-node7
```

## Usage

Read ["Configuring Babel 6" article](http://www.2ality.com/2015/11/configuring-babel6.html)
for more information about babel@6 configuration.

### Node run

```shell
node script.js
```

### Via `.babelrc` (recommended)

**.babelrc**

```json
{
  "presets": ["es2017-node7"]
}
```

### Via CLI

```js
babel script.js --presets es2017-node7
```

### Via Node API

```js
require('babel-core').transform('code', {
  presets: ['es2017-node7'],
})
```

## Credits

* Inspired by [babel-preset-es2015-node6](https://github.com/jhen0409/babel-preset-es2015-node6)

## License

[MIT](LICENSE.md)
