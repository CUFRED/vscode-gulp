# [Gulp - VS Code](https://github.com/Tanato/vscode-gulp)

## Installation

Just type `cmd+p`/`ctrl+p` to bring up the command pallete and pick `>Extension Installer` from the dropdown, type `gulp` and select the extension, restart VSCode and you are all set.

## Snippets

#### gulpvar
```
var gulp = require('gulp-name');
```

#### pipe | gulppipe
```
.pipe(name('file'))
```

#### gulpsrc - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpsrcglobs-options)
```
gulp.src('scriptFiles')
  .pipe(name('file'))
```

#### gulptask - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulptaskname-deps-fn)
```
gulp.task('name',['tasks'], function() {
    // content
});
```

#### gulpdest - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpdestpath)
```
.pipe(gulp.dest('folder'));
```

#### gulpwatch - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpwatchglob-opts-tasks)
```
gulp.watch('file', ['tasks']);
```

#### gulpwcb - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpwatchglob-opts-cb)
```
gulp.watch('file', function(event) {
  console.log(' File '+event.path+' was '+event.type+', running tasks...');
});
```

** Enjoy!**