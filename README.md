unite-xcode_complete
====================

unite source for xcode (iOS) complete

## .vimrc sample

```vim
NeoBundle 'https://github.com/tokorom/unite-xcode_complete'

autocmd FileType objc inoremap <silent><expr> <C-x><C-o>
  \ unite#start_complete(
  \   ['xcode_complete'],
  \   {
  \     'start_insert' : 1,
  \     'input' : unite#sources#xcode_complete#get_cur_text(),
  \   }
  \ )
```
