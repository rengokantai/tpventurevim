# tpventurevim
##2. Digging Deeper
###1 Search
delete until first searched word
```
d
/word
enter
```
insert.
```
c
/word
enter
```
###2 Replace
```
:s/a/b    //current line first occurance
:%s/a/b    //all lines first occurance
```
####05:29
v //visual mode
shift v //visual line mode





###4 Advanced Movement
```
ctrl d //move half screen down
ctrl u //move half screen up
ctrl f //move full screen down(forward)
ctrl b //move full screen up(backward)
```


















###5 Using the Command Line Directly From Vim
```
read(r) !curl http://
```
set file type
```
set ft=javascript
```

###6 Buffers
```
:ls  //list all buffers
:bp  //previuos buffer
:b#  //last buffer we were visiting
:bnext //next
```
##4. Customization
###3 Themes
####01:29
```
:colo delek
```
set background
```
:set bg=light
```
install theme
```
git clone --depth 1 https://github.com/vim-scripts/Zenburn
```
vim
```
:call pathogen#infect()
```

open the file
```
:e Zenburn/colors/zenburn.vim
```



###4 Mappings
```
:map ,rs :bundle exec rspec<CR>     //CR = enter key
```
next time, set
```
,rs
```
vmap
```
:vmap ,cs :!coffee -s -c<CR>
```

imap
```
:imap <Tab> <C-n>
```

map a shortcut to another shortcut (shift tab->ctrl p)
```
:imap <S-Tab> <C-p>
```
