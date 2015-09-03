# Sensible Config

Sensible configuration files for professional front-end development.

## ESLint

A `.eslintrc` file that enforces AirBnB style JavaScript linting and code style.

Install eslint, babel-eslint and eslint-config-airbnb in your project.

```sh
npm install --save-dev eslint-config-airbnb babel-eslint
```

In order to use it in your editor just install and activate the respective
ESLint plugin. There are very excellent plugins for [Atom](https://github.com/AtomLinter/linter-eslint), [Webstorm](https://www.jetbrains.com/webstorm/help/eslint.html),
[SublimeText](https://github.com/roadhump/SublimeLinter-eslint) and
[Vim](http://www.vim.org/scripts/script.php?script_id=2736).

You can also use [Grunt](https://github.com/sindresorhus/grunt-eslint) or
[Gulp](https://github.com/adametry/gulp-eslint) or the
[cli](https://github.com/eslint/eslint) directly to lint your code.

### The Code Style

It is [AirBnB's JavaScript code style](https://github.com/airbnb/javascript) without the ReacJS specific things.

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
or clone this repository with Git and then copy all configuration files from
the `config-files` folder into the root of you project and tweak as needed.

### Add the configuration files to your project with cURL

Run this on the terminal in your project directory:

```sh
curl -fsSL http://git.io/vfQKP | tar -xz --strip-components 2
```

Tweak as needed.

# License

MIT © [Kahlil Lechelt](http://kahlil.info)
