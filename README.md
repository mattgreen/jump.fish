# jump.fish

`jump` is a fish package that enables you to easily jump between projects. For example, to jump to the `blog` project:

    $ j blog

`jump` assumes that projects are stored under a configurable root project directory. Thus, when you enter `j blog`, it expands it to `cd $j_path/blog`.

Unlike other takes on project switching, **j has no training period**, nor does it rely on fancy algorithms that may occasionally surprise you. Instead, `jump` is carried by it's support for **tab completions** out of the box. Entering `j dotfiles/fish/func` <kbd>Tab</kbd> completes to `dotfiles/fish/functions`.

## Installation

Install with [Fisher](https://github.com/jorgebucaran/fisher)

```console
fisher add mattgreen/jump.fish
```

If you aren't using Fisher, you may copy the contents of the `completions`, `conf.d`, and `functions` directories to your fish configuration.

## Configuration
Update `~/.config/fish/config.fish` with your project directory root:
```fish
# Set root path for jump.fish
set -g j_path "$HOME/Code"
```

`$j_path` defaults to `$HOME/Projects`. Additionally, prefer using `$HOME` to specify your home directory in lieu of `~`.

## License
MIT