# Poppy [demo](http://dfcreative.github.io/poppy)

Poppy is a versatile and reliable popups constructor. It provides basic kinds of popups:

* overlay
* tooltip
* dropdown
* notifier
* popover
* slide-nav
* modal
* balloon

With poppy you can easily build your own popups as well.

[![NPM](https://nodei.co/npm/poppy.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/poppy/)


## Getting started

### Install

Get the latest version from [builds](todo) or [CDN](todo). Insert script on the page:

```html
<script src="CDN/poppy.js"></script>
```

Poppy is also available as a component for browserify, component or duo:

`$ npm install poppy`

```js
var Dropdown = require('poppy/dropdown');
```

### Use

Create new dropdown instance:

```js
var dropdown = new Dropdown({
	target: document.queryElement('#dropdown'),
	content: '<ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul>'
});
```


## Options

| Parameter | Type | Default | Description |
|----|----|----|----|
| `target` | _selector_, _Element_, _NodeList_, `undefiend`  | `undefined` | A target or list of targets which by click show the popup container. Can vary depending on poppy type. |
| `content` | _string_, _Element_, _function_ | `undefined` | Content to show within the container. If function defined—it will be invoked and result considered as content. |
| `contentType` | _string_ | `element` | <dl><dt>`'element'`</dt><dd>Show other element in the container</dd><dt>`'text'`</dt><dd>Show content as plain text</dd><dt>`'html'`</dt><dd>Show content as inner html</dd></dl> |
| `containerClass` | _string_ | `''` | A class to add to the popup container |
| `holder` | _selector_, _Element_ | `<body>` | A holder of container |
| `tip` | `'top'`, `'left'`, `'bottom'`, `'right'`, `undefined` | `false` | Show tip — a little triangle on the edge of the container. |
| `tipAlign` | _string_, _number_ | `'center'` | Tip alignment relative to the container. |
| `single` | _bool_ | `false` | Hide other containers when this one becomes visible |


## API

| Property/method | Type | Default | Description |
|----|----|----|----|
| `show()` |  |  |  |
| `hide`() |  |  |  |
| `enable()` |  |  |  |
| `disable()` |  |  |  |
| `container` |  |  |  |
| `state` |  |  |  |


## Events

| Property/method | Type | Default | Description |
|----|----|----|----|
| `beforeShow` |  |  |  |
| `show` |  |  |  |
| `beforeHide` |  |  |  |
| `hide` |  |  |  |
| `enable` |  |  |  |
| `disable` |  |  |  |


## License

MIT
