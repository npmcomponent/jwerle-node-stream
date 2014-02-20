*This repository is a mirror of the [component](http://component.io) module [jwerle/node-stream](http://github.com/jwerle/node-stream). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/jwerle-node-stream`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
node-stream
======

DOM Nodes as streams

## install

```sh
$ component install jwerle/node-stream
```

## usage

```html
<div id="element">
</div>
```

```js
var NodeStream = require('node-stream')
var node = document.getElementById('element');
var stream = NodeStream(node);

stream.on('data', function (chunk) {
  console.log(chunk); // 'beep'
});

stream.write('beep');
console.log(node.innerHTML); // 'beep'
```

## license

MIT
