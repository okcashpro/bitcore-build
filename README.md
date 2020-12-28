# okcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install okcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var okcoreTasks = require('okcore-build');

okcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var okcoreTasks = require('okcore-build');
okcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/okcashpro/okcore) on the main okcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/okcashpro/okcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2020 The Okcash Developers
