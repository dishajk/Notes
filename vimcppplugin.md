1. YouCompleteMe Vim plugin was installed
2. 'sudo apt-get install build-essential cmake python3-dev'
3. 'cd ~/.vim/bundle'
4. 'git clone https://github.com/ycm-core/YouCompleteMe.git'
5. 'cd YouCompleteMe'
5. 'git submodule update --init --recursive'
6. './install.py --clang-complete'
7. edit '~/.vim/bundle/YouCompleteMe/.ycm_extra_conf.py' to add 
```
def Settings(**kwargs ):
  return {
    'flags': [ '-x', 'c++', '-Wall', '-Wextra', '-Werror' ],
  }
```
8. append the following line to '~/.vimrc'
```
let g:ycm_global_ycm_extra_conf = '~/.vim/bundle/YouCompleteMe/.ycm_extra_conf.py'
```     
