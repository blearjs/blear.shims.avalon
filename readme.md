# blear.shims.avalon

[![npm module][npm-img]][npm-url]
[![build status][travis-img]][travis-url]
[![coverage][coveralls-img]][coveralls-url]

[travis-img]: https://img.shields.io/travis/blearjs/blear.shims.avalon/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/blearjs/blear.shims.avalon

[npm-img]: https://img.shields.io/npm/v/blear.shims.avalon.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/blear.shims.avalon

[coveralls-img]: https://img.shields.io/coveralls/blearjs/blear.shims.avalon/master.svg?style=flat-square
[coveralls-url]: https://coveralls.io/github/blearjs/blear.shims.avalon?branch=master

# 分类
- 经典版 `src/classical.js`，兼容到 IE6
- 现代版 `src/modern.js`，只兼容高级浏览器

# 定制
相比原始的 avalon，修改了以下内容

- `define` 的 `$id` 参数为 DOM 元素的 ID
- 增加了 `$el` 属性，指向当前 DOM 元素
- 增加了 `$destroy` 方法，用于销毁 vm
- 删除了 `date`、`number`、`currency` 过滤器

# 使用
```
<div id="demo"></div>

avalon.define({
    $id: 'demo'
});
```

