# gulp-angular-architecture-graph  [![Dependency Status][depstat-image]][depstat-url] [![devdependencies][devdepstat-image]][devdepstat-url]

[depstat-url]: https://david-dm.org/vogloblinsky/gulp-angular-architecture-graph
[depstat-image]: https://david-dm.org/vogloblinsky/gulp-angular-architecture-graph.svg
[devdepstat-url]: https://david-dm.org/vogloblinsky/gulp-angular-architecture-graph#info=devDependencies
[devdepstat-image]: https://david-dm.org/vogloblinsky/gulp-angular-architecture-graph/dev-status.png

Generate modules dependencies graph. Port of https://github.com/lucalanca/grunt-angular-architecture-graph

## Getting Started

This plugin requires Gulp `~3.8.7`

If you haven't used [Gulp](http://gulpjs.com/) before, be sure to check out the [Getting Started](https://github.com/gulpjs/gulp/blob/master/docs/getting-started.md) guide, as it explains how to create a [Gulpfile](https://github.com/gulpjs/gulp#sample-gulpfilejs) as well as install and use Gulp plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install gulp-angular-architecture-graph --save-dev
```

Once the plugin has been installed, it may be injected inside your Gulpfile with this line of JavaScript:

```js
var ngGraph = require('gulp-angular-architecture-graph');

gulp.task('default', function(){
    gulp.src('src/*.js')
        .pipe(ngGraph({
            dest: 'architecture'
        }));
});
```

## The task

#### OS X

***Requirements***

- [**graphviz**](http://www.graphviz.org/)

if running OS X and using homebrew, simply execute:

```
 brew install graphviz
```

#### Windows 7

***Requirements***

The windows installer of graphviz: [graphviz-X.XX.msi](http://www.graphviz.org/Download..php), remember to set the Path and point it to your bin directory. e.g. ```C:\Program Files (x86)\GraphvizX.XX\bin```.

#### Manjaro 0.8.11 (arch linux)

***Requirements***

Install via `yaourt` the graphviz package e.g.: `yaourt graphviz`.

#### General

***Requirements***

https://github.com/lucalanca/angular-architecture-graph