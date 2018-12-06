
> Strip `console`, `alert`, and `debugger` statements from JavaScript code with [`strip-debug-option`](https://github.com/SamLiu001/strip-debug-option)


## Install

```
$ npm install --save-dev gulp-strip-debug-option
```


## Usage

```js
const gulp = require('gulp');
const stripDebug = require('gulp-strip-debug');

const option={
	skipDebugger:false,
	skipConsole:false,
	skipAlert:false
}

gulp.task('default', () =>
	gulp.src('src/app.js')
		.pipe(stripDebug(option))
		.pipe(gulp.dest('dist'))
);
```


## License

MIT
