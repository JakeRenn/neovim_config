## Install 

Install [neovim](https://github.com/neovim/neovim/wiki/Installing-Neovim) and [vim-plug](https://github.com/junegunn/vim-plug). 

Follow the official instructions to install `neovim` and run the following command to install `vim-plug`

```sh
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

A few more commands

```sh
mkdir -p ~/.config
git clone https://github.com/JakeRenn/neovim_config.git ~/.config/nvim
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


