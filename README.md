call plug#begin('~/.vim/plugged')

"Tema vscode
Plug 'tomasiser/vim-code-dark'
Plug 'NLKNguyen/papercolor-theme'

"fecha () {} [] auto
Plug 'jiangmiao/auto-pairs'

"Navegação rápida no arquivo
Plug 'easymotion/vim-easymotion'

"Plugin para o explorador de arquivos
Plug 'preservim/nerdtree'

"Barra de status
Plug 'vim-airline/vim-airline'
Plug 'vim-airline/vim-airline-themes'

"Manipulação de 'surroudings' (aspas, parênteses etc.)
Plug 'tpope/vim-surround'

"Comentar e descomentar linhas
Plug 'tpope/vim-commentary'

"Histórico visual de alterações
Plug 'mbbill/undotree'

"Integração com Git
Plug 'tpope/vim-fugitive'

"Syntax / linguagens
Plug 'sheerun/vim-polyglot'

"Qualidade de vida
Plug 'tpope/vim-surround'
Plug 'tpope/vim-commentary'

"GitHub
Plug 'tpope/vim-fugitive'
Plug 'airblade/vim-gitgutter'

call plug#end()

"Keymap
"Easymotion -> \\w para pular por palavras
map <Leader>w <Plug>(easymotion-w)
map <F3> :NERDTreeToggle<CR>
map <F5> :UndotreeToggle<CR>

nnoremap <C-q> :q<CR>

nnoremap <C-Left>	<C-w>h
nnoremap <C-Down>	<C-w>j
nnoremap <C-Up>	<C-w>k
nnoremap <C-Right>	<C-w>l

nnoremap <C-S-Left>	<C-w>H
nnoremap <C-S-Down>	<C-w>J
nnoremap <C-S-Up>	<C-w>K
nnoremap <C-S-Right>	<C-w>L

nnoremap <A-h> <C-w>>
nnoremap <A-j> <C-w><
nnoremap <A-l> <C-w>-
nnoremap <A-k> <C-w>+
"Habilita a barra de status do airline
set encoding=utf-8
set laststatus=2
let g:airline_powerline_fonts = 0
let g:airline_symbols_ascii = 1

"Desliga o statusline padrão do Vim
set noshowmode
syntax enable
set background=dark
colorscheme codedark
