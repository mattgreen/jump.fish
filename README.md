# jump.fish

`jump` is a fish package that enables you to easily jump between projects. For example, to jump to the `blog` directory:

    $ j blog

`jump` assumes that projects are stored under a configurable root project directory. Thus, when you enter `j blog`, it expands it out to `cd $j_path/blog`.

Unlike other takes on project switching, **j has no training period**, nor does it rely on fancy algorithms. Instead, `j` is carried by it's support for **tab completions** out of the box. It works as you'd expect:

    $ j dotfiles/fish/func<kbd>Tab</kbd> # expands to dotfiles/fish/functions

## Installation

Install with [Fisher](https://github.com/jorgebucaran/fisher)

```console
fisher add mattgreen/jump.fish
```

## Configuration
Update `~/.config/fish/config.fish` with your project directory:
```fish
set -g j_path ~/Code
```

## License
MIT