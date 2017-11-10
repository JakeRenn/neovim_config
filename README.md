## Prerequistes

Follow the instructions from official docs in [neovim](https://github.com/neovim/neovim/wiki/Installing-Neovim) to install `nvim` software.

Install [vim-plug](https://github.com/junegunn/vim-plug) Plugin Manager. For Unix and neovim user, run the following command
```sh
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
If you need more information about other platform or other details, you may read the [official docs](https://github.com/junegunn/vim-plug) here.

## Installation

Make the directory
```sh
mkdir -p ~/.config
```

Clone this repository into your `~/.config` directory with the following command
```sh
git clone https://github.com/JakeRenn/neovim_config.git ~/.config/nvim
```

Install the Plugins
```sh
nvim +PlugInstall
```


## Autocompelete
To enable autocompeletion, we need a few more steps.

Clone the [deoplete.nvim](https://github.com/Shougo/deoplete.nvim) into `~/.config/nvim`

```sh
cd ~/.config/nvim && git clone https://github.com/Shougo/deoplete.nvim.git
```

Compile the project.
```sh
cd deoplete.nvim && make
```

**Note** If if fail to load `deoplete`, please enter `nvim` and type `:UpdateRemotePlugins` in normal mode.


