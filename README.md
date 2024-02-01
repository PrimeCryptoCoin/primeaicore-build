# primeaicore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install primeaicore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var primeaicoreTasks = require('primeaicore-build');

primeaicoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var primeaicoreTasks = require('primeaicore-build');
primeaicoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/PrimeCryptoCoin/primeaicore-lib) on the main primeaicore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/PrimeCryptoCoin/primeaicore-lib/blob/master/LICENSE).

