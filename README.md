" Define o início da seção de plugins
call plug#begin('~/.vim/plugged')

"Tema vscode
Plug 'tomasiser/vim-code-dark'
Plug 'NLKNguyen/papercolor-theme'
"Plugin para o explorador de arquivos
Plug 'preservim/nerdtree'

"Manipulação de 'surroudings' (aspas, parênteses etc.)
Plug 'tpope/vim-surround'

"Comentar e descomentar linhas
Plug 'tpope/vim-commentary'

"Histórico visual de alterações
Plug 'mbbill/undotree'

"Integração com Git
Plug 'tpope/vim-fugitive'

" Adicione seus plugins aqui

" Define o fim da seção de plugins
call plug#end()

map <F3> :NERDTreeToggle<CR>
map <F5> :UndotreeToggle<CR>

"Habilita a barra de status do airline
let g:airline_powerline_fonts = 1

"Desliga o statusline padrão do Vim
set noshowmode
syntax enable
set background=dark
colorscheme codedark
