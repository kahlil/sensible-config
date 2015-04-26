# Sensible Config

Sensible configuration files for professional front-end development.

## ESLint

A `.eslintrc` file that enforces sensible linting and code style.

Install ESLint globally on your system:

```sh
npm install -g eslint
```

In order to use it in your editor just install and activate the respective
ESLint plugin. There are very excellent plugins for [Atom](https://github.com/AtomLinter/linter-eslint), [Webstorm](https://www.jetbrains.com/webstorm/help/eslint.html),
[SublimeText](https://github.com/roadhump/SublimeLinter-eslint) and
[Vim](http://www.vim.org/scripts/script.php?script_id=2736).

You can also use [Grunt](https://github.com/sindresorhus/grunt-eslint) or
[Gulp](https://github.com/adametry/gulp-eslint) or the
[cli](https://github.com/eslint/eslint) directly to lint your code.

### The Code Style

My code style includes the following things:

* semicolons (which you can turn off by changing the `semi` setting in the `.eslintrc`)
* 2 spaces indentation
* no multiple line strings (use templates!)
* every variable get a var, none of that weird comma bizzniz!
* no quoted keys in objects
* no trailing whitespace
* definitely use curly braces
* `var self = this;`
* single quotes for strings
* [and more ...](https://github.com/distilledhype/sensible-config/blob/master/.eslintrc)

_Highlight:_ the environments `browser`, `node`, `jquery`, `jasmine` and `mocha`
are all turned on by default so ESLint allows all the necessary globals.

## EditorConfig

The `.editorconfig` file mirrors the settings given in the `.eslintrc`. Make sure
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

The `.gitattributes` file just makes sure that if Git decides that the content
is text, its line endings are normalized to LF on checkin.

## How to Use

There are two ways to get these files into your project cleanly.

### Add Manually

Download [the master zip](https://github.com/distilledhype/sensible-config/archive/master.zip),
then copy all configuration files into the root of you project and tweak as needed.

### Merge with Git

If you want to merge the sensible-config files into your project with Git you can do
that by adding this repo as a remote repo in your project, fetch that repo and
merge master:

```sh
git remote add sensible-config https://github.com/distilledhype/sensible-config.git
git fetch sensible-config
# Make sure you merge with care and don't overwrite your README.md.
git merge sensible-config/master
# Delete the sensible-config remote if you want
git remote delete sensible-config
```

Tweak as needed.

# License

MIT © [Kahlil Lechelt](http://kahlil.info)
