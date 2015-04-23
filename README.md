# Sensible Config

Essential configuration files for professional front-end development.

## JSCS

A `.jscsrc` file that enforces a common sense code style.
In order to use it in your editor just install and activate the respective
JSCS plugin.

In order to use it with grunt use the `grunt-jscs` plugin.
In order to use it with gulp use the `gulp-jscs` plugin.
In order to use it on the command line install JSCS with `npm i -g jscs`.  

### The Code Style

My code style includes the following things:

* semicolons (which you can turn off by changing just one line in the .jscsrc)
* 2 spaces indentation
* no anonymous functions aloud, they all have to have a name
* no multiple line strings (use templates!)
* every variable get a var, none of that weird comma bizzniz!
* no quoted keys in objects
* 80 characters line length
* no trailing whitespace
* definitely use curly braces
* `var self = this;`
* single quotes for strings
* and more ...

## JSHint

The `.jshintrc` file is quite small since I am not turning off any of the
stricter options and they removed all the code style options while referring
to to JSCS for that.

It should do a good job linting your client side code. You might have to add
or change a couple of options for server side JavaScript.

_Highlight:_ the `browserify` option is turned on by default so you won't have any
problems working with CommonJS in your client side code.

## EditorConfig

The `.editorconfig` file mirrors the settings given in the `.jscsrc`. Make sure
you have the respective EditorConfig plugin installed in your editor.

## Gitignore

The `.gitignore` file has been generated with the awesome [gitignore.io](http://gitignore.io)
service and ignores common patterns for:

* OS X
* Linux
* Windows
* SublimeText
* Vim
* Webstorm, PHPStorm etc.
* Node
* Grunt
* Bower
* Sass

Tweak as needed.

## License

MIT © [Kahlil Lechelt](http://kahlil.info)
