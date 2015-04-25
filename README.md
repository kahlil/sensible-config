# Sensible Config

Essential configuration files for professional front-end development.

## ESLint

A `.eslintrc` file that enforces sensible linting and code style.
In order to use it in your editor just install and activate the respective
ESLint plugin.

* you can use it with [Grunt](https://github.com/sindresorhus/grunt-eslint)
* you can use it with [Gulp](https://github.com/adametry/gulp-eslint)
* you can use it just as a [cli](https://github.com/eslint/eslint)

### The Code Style

My code style includes the following things:

* semicolons (which you can turn off by changing just one line in the .jscsrc)
* 2 spaces indentation
* no multiple line strings (use templates!)
* every variable get a var, none of that weird comma bizzniz!
* no quoted keys in objects
* no trailing whitespace
* definitely use curly braces
* `var self = this;`
* single quotes for strings
* and more ...

_Highlight:_ the environments `browser`, `node`, `jquery`, `jasmine` and `mocha`
are all turned on by default so ESLint allows all the necessary globals.

## EditorConfig

The `.editorconfig` file mirrors the settings given in the `.jscsrc`. Make sure
you have the respective EditorConfig plugin installed in your editor.

## Gitignore

The `.gitignore` file has been generated with the awesome
[gitignore.io](http://gitignore.io) service and ignores common patterns for:

* OS X
* Linux
* Windows
* SublimeText
* Vim
* Webstorm, PHPStorm
* Node
* Grunt
* Bower
* Sass

## Gitattributes

The `.gitattributes` file just makes sure that all text files get normalized to
LF on checkin.

## How to Use

Copy all configuration files into the root of you project and tweak as needed.

# License

MIT © [Kahlil Lechelt](http://kahlil.info)
