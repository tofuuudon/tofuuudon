# Hey, I'm Mikey 👋

- 🧑‍🎓 Graduated with a 1st, I'm now embarking on a Master's in Applied AI and Data Science.
- 🌱 I’m currently learning more about back-end development, native frameworks, and data science.
- 💻 HTML, CSS/SCSS, Javascript/Typescript, PHP/Laravel, Python, R, C#, Vue/Vuex/Nuxt, React/Next/Native, Laravel, Node, Docker, Cypress, Jest.
- 💖 In love with VIM.
- 🍣 Sushi is my go-to for lunch-breaks.

## My VIM setup

```vim
set number

call plug#begin('~/.vim/plugged')
Plug 'vim-airline/vim-airline'
Plug 'vim-airline/vim-airline-themes'
Plug 'sheerun/vim-polyglot'
Plug 'joshdick/onedark.vim'
Plug 'prettier/vim-prettier', { 'do': 'npm install' }
Plug 'jiangmiao/auto-pairs'
Plug 'wincent/command-t'
Plug 'junegunn/fzf', { 'do': { -> fzf#install() } }
Plug 'junegunn/fzf.vim'
Plug 'jdhao/better-escape.vim'
Plug 'w0rp/ale'
Plug 'machakann/vim-highlightedyank'
Plug 'mcchrish/nnn.vim'
Plug 'pechorin/any-jump.vim'
Plug 'kshenoy/vim-signature'
Plug 'valloric/youcompleteme'
Plug 'airblade/vim-gitgutter'
Plug 'kristijanhusak/vim-js-file-import', {'do': 'npm install'}
Plug 'tpope/vim-fugitive'
call plug#end()

"Vundle installation
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
Plugin 'VundleVim/Vundle.vim'
Plugin 'ycm-core/YouCompleteMe'
Plugin 'alvan/vim-closetag'
call vundle#end()
filetype plugin indent on

"Theme
colorscheme onedark
let g:airline_powerline_fonts = 1
syntax on
set re=0

let g:closetag_filenames = '*.html,*.xhtml,*.phtml,*.tsx,*.jsx'

"Disables YouCompleteMe preview window
set completeopt-=preview
nmap <leader>fw <Plug>(YCMFindSymbolInWorkspace)
nmap <leader>fd <Plug>(YCMFindSymbolInDocument)

"NNN mapping
let g:nnn#action = {
      \ '<c-t>': 'tab split',
      \ '<c-x>': 'split',
      \ '<c-v>': 'vsplit' }

"Any jump for ref and def 
let g:any_jump_disable_default_keybindings = 1
nnoremap <leader>ff :AnyJump<CR>
xnoremap <leader>ff :AnyJumpVisual<CR>
nnoremap <leader>jb :AnyJumpBack<CR>
nnoremap <leader>jl :AnyJumpLastResults<CR>

"Prettier
autocmd BufWritePre * PrettierAsync

"ESC
let g:better_escape_interval = 200
let g:better_escape_shortcut = 'jj'
```
