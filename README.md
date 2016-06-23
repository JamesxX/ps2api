Pointshop 2 API (PS2API)
=========

A minimal node module providing utility methods to read and write data from a MySQL server containing pointshop 2 data. Get the module here [![npm version](https://badge.fury.io/js/ps2api.svg)](https://badge.fury.io/js/ps2api)


## Installation

```shell
npm install ps2api --save
```

## Usage

```js
var psapi = require('p2sapi');

var Pointshop = new psapi.Connection( '0.0.0.0', 'root', '', 'pointshop_stuff' );
Pointshop.Event.on('connected', function( obj ){
	obj.getUser(123456789).giveItem('MyAwesomeItem');
});
Pointshop.Event.on('error', function(error){
	console.log( error );
});
```

## Tests

```shell
npm test
```

## Contributing

In lieu of a formal styleguide, take care to maintain the existing coding style.
Add unit tests for any new or changed functionality. Lint and test your code.

## Release History

* 0.0.1 Initial release
