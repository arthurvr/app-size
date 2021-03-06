# app-size [![Build Status](https://travis-ci.org/gillstrom/app-size.svg?branch=master)](https://travis-ci.org/gillstrom/app-size)

> Get an app's size in byte (OS X)


## Install

```
$ npm install --save app-size
```


## Usage

```js
var appSize = require('app-size');

appSize('Safari', function (err, size) {
	console.log(size);
	// => 34058118
});

appSize('/Applications/Safari.app', function (err, size) {
	console.log(size);
	// => 34058118
});

appSize('com.apple.Safari', function (err, size) {
	console.log(size);
	// => 34058118
});
```


## CLI

```
$ npm install --global app-size
```

```
$ app-size --help

  Examples
    $ app-size Safari
    $ app-size /Applications/Safari.app
    $ app-size com.apple.Safari
```


## License

MIT © [Andreas Gillström](https://github.com/gillstrom)
