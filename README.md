# `~/.*`

My dotfiles.

## Plugin manager

### oh-my-zsh

```sh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### vim-plug

#### Linux

```sh
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

#### PowerShell

```powershell
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni $HOME/vimfiles/autoload/plug.vim -Force
```

## Alternative tools

|  TRADITIONAL  |  NEW  |
| ---- | ---- |
|  find  |  [fd](https://github.com/sharkdp/fd)  |
|  cat  |  [bat](https://github.com/sharkdp/bat)  |
