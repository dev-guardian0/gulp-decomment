gulp-decomment
==============

Uses [decomment] to remove comments from JSON, JavaScript, CSS, HTML, etc.

[![Build Status](https://travis-ci.org/vitaly-t/gulp-decomment.svg?branch=master)](https://travis-ci.org/vitaly-t/gulp-decomment)
[![Coverage Status](https://coveralls.io/repos/vitaly-t/gulp-decomment/badge.svg?branch=master)](https://coveralls.io/r/vitaly-t/gulp-decomment?branch=master)

## Installing

```
$ npm i gulp-decomment
```

## Testing

```
$ npm test
```

Testing with coverage:
```
$ npm run coverage
```

## Usage

```js
const gulp = require('gulp');
const decomment = require('gulp-decomment');

gulp.task('default', () => 
    gulp.src('input.js')
    .pipe(decomment({trim: true}))
    .pipe(gulp.dest('dest'))
);
```

