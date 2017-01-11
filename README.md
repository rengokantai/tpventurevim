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



###3 Macros and Registers
####01:00
ctrl g //see status of file

####02:00
delete line and below
```
dj
```

create a macro called a
```
qa
```
####05:43
end recording macro
```
q
```
check all registers
```
:registers
:reg
```

execute macro
```
@a
```
@ means last macro used, here
```
200@@ = 200@a
```














###4 Advanced Movement
```
ctrl d //move half screen down
ctrl u //move half screen up
ctrl f //move full screen down(forward)
ctrl b //move full screen up(backward)
```
go to middle of screen
```
M
```
go to top of window
```
H
```
go to buttom of window
```
L
```
3 lines above bottom of the window
```
3L
```

set currentline(cursor) stay on the top
```
zt
```
conversely
```
zb
```
middle
```
zz
```


####05:00
set register(marker)
```
ma   //set marker name a
```

```
'a   //go to marker name a
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

##3. Vim as an Extension of Vi
###1 Windows and Tabs
```
vsplit filename
```

```
ctrl w +  //add height of window ( vertical)
ctrl w -  //reduce height of window ( vertical)
ctrl w >  //add width of window (horizontal)
ctrl w <  //reduce width of window (horizontal)
```

equal size all windows
```
ctrl w =
```


```
:sb2   //open buffer number x
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
