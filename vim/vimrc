call plug#begin('~/.vim/plugged')
  Plug 'neoclide/coc.nvim', {'branch': 'release'}
  Plug 'lepture/vim-jinja'
  Plug 'editorconfig/editorconfig-vim'
  Plug 'tyru/eskk.vim'
call plug#end()

syntax on

set nowritebackup
set nobackup
set noswapfile
set number              

setglobal ignorecase
setglobal smartcase
setglobal incsearch
setglobal hlsearch            
set wrap                
set textwidth=0         
hi Comment ctermfg=green

let mapleader = "\<Space>"
nnoremap <Leader>w :w<CR>
nnoremap <Leader>h :<C-u>help<Space>
nnoremap <Leader>hh :<C-u>help<Space><C-r><C-w><Enter>
nnoremap <Leader>. :edit $MYVIMRC<CR>
nnoremap <Leader>s. :source $MYVIMRC<CR>
vnoremap <silent> * "vy/\V<C-r>=substitute(escape(@v, '\/'), "\n", '\\n', 'g')<CR><CR>
nnoremap j gj
nnoremap k gk
nmap <silent> <Esc><Esc> :nohlsearch<CR>


" indent
set tabstop=4
set shiftwidth=4
set softtabstop=4
set expandtab
set autoindent
set smartindent

" status line
set statusline=%F
set statusline+=%m
set statusline+=%r
set statusline+=%h
set statusline+=%w
set statusline+=%=
set statusline+=[ENC=%{&fileencoding}]
set statusline+=[LOW=%l/%L]
set laststatus=2

" filetype
au BufNewFile,BufRead *.njk set ft=jinja

" skk
let g:eskk#directory = "~/.config/eskk"
let g:eskk#dictionary = { 'path': "~/.config/eskk/my_jisyo", 'sorted': 1, 'encoding': 'utf-8',}
let g:eskk#large_dictionary = {'path': "~/.config/eskk/SKK-JISYO.L", 'sorted': 1, 'encoding': 'euc-jp',}

" GoTo code navigation.
nmap <silent> gd <Plug>(coc-definition)
nmap <silent> gy <Plug>(coc-type-definition)
nmap <silent> gi <Plug>(coc-implementation)
nmap <silent> gr <Plug>(coc-references)
