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
Modos do Vim

O Vim tem alguns modos:

    Normal mode: para se movimentar pelo texto
    Insert mode: para escrever no texto
    Visual mode: para selecionar parte do texto
    Command mode: para dar algum comando ao Vim

Comandos básicos no modo normal

    esc: sair do modo atual e ir para o modo de comando
    j: mover o cursor para baixo
    k: mover o cursor para cima
    h: mover o cursor para a esquerda
    l: mover o cursor para a direita
    ctrl i: entrar no modo de edição no caracter em que está
    esc: sair do modo atual e ir para os comandos
    shift a: entrar no modo de edição no final da linha
    shift o: entra no modo de edição em uma nova linha abaixo da atual
    gg: ir para o início do arquivo
    shift g: ir para o final do arquivo
    w: pular uma palavra para frente
    b: pular uma palavra para trás
    ctrl ]: pular um bloco de código para baixo
    ctrl [: pular um bloco de código para cima
    y: copiar código
    c: recortar código
    p: colar código um caractere depois do atual
    x: deletar caractere
    dd: deletar linha
    ctrl u: desfazer
    ctrl r: refazer
    shift o: abre uma nova linha de edição empurrando para baixo o código da linha

Comandos no modo de comando

Entramos nesse modo depois de dar um esc. Perceba que aqui nós precisamos digitar dois pontos para dar o comando e dar enter no final. Aqui os comandos aparecem sendo digitados no canto inferior da tela (lá no finzinho).

Vim image

    :q: sair do arquivo atual
    :q!: saída forçada do arquivo atual
    :w: salvar
    :wq: salvar e sair

Comandos no modo visual

Com o v entramos no visual mode, e com os comandos do modo normal movemos o cursor para que selecione o texto que queremos. Ficará um VISUAL no canto inferior.

Vim image

    x: deleta o que está selecionado
    y: copia o que está selecionado
    s: entra no modo de edição substituindo o que tinha antes
    c: recorta o código selecionado

Para copiar o código selecionado em algum lugar, dê um esc para voltar ao modo normal e depois um p (paste) no local desejado.
Comandos do Vundle e do plugin NERDTree

Para instalar os plugins que você definiu no seu .vimrc entre no Vim e, no modo de comando, digite:



:PluginInstall


Vai aparecer uma telinha como essa:

Vim image

É só dar esc, depois :q e enter para sair. Para desinstalar um plugin delete a linha no .vimrc e depois faça o mesmo esquema só que com :PluginClean.

Para acessar a árvore de comandos que eu instalei, vá para o modo de comando e digite:



:NERDTree


Você pode navegar na NERDTree como no normal mode. Para abrir uma pasta pressione o, para fechá-la, pressione novamente.

Para abrir um arquivo do lado pressione o no arquivo. Para abrir outro arquivo na vertical, dividindo a tela com um arquivo já aberto, pressione i.

Para rodar entre os arquivos abertos e a árvore de arquivos pressione ctrl w e mais uma das teclas principais de navegação (h, j, k, l).

Cada plugin tem uma documentação e você deve ler cada uma delas para entender o que fazer. Não tem para onde correr!
