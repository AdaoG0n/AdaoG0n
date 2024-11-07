```
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

```sh
  1 " configurações essenciais
  2 set nocompatible              " be iMproved, required
  3 filetype off                  " required
  4 set rtp+=~/.vim/bundle/Vundle.vim
  5 " início da chamada de plugins
  6 call vundle#begin()
  7 
  8 Plugin 'VundleVim/Vundle.vim'
  9 Plugin 'scrooloose/nerdtree'
 10 Plugin 'majutsushi/tagbar'
 11 Plugin 'tpope/vim-surround'
 12 Plugin 'scrooloose/syntastic'
 13 Plugin 'jiangmiao/auto-pairs'
 14 Plugin 'morhetz/gruvbox'
 15 Plugin 'valloric/youcompleteme'
 16 
 17 " fim da chamada de plugins
 18 call vundle#end()            " required
 19 filetype plugin indent on    " required
 20 
 21 " configurações básicas do Vim
 22 set number
 23 set linebreak
 24 set showbreak=+++
 25 set textwidth=100
 26 set showmatch
 27 set hlsearch
 28 set smartcase
 29 set ignorecase
 30 set incsearch
 31 set autoindent
 32 set shiftwidth=2
 33 set smartindent
 34 set smarttab
 35 set softtabstop=2
 36 set undolevels=1000
 37 set background=dark
 38 set backspace=indent,eol,start
 39 colorscheme gruvbox
~                        
```

```
:PluginInstall
```
