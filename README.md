# dottmux tmux config

My personal tmux settings. Contains custom bindings and plugins.

## Installation

```bash
git clone https://github.com/steven-nichols/dottmux.git ~/.tmux
ln -s ~/.tmux/.tmux.conf ~/.tmux.conf
```

Now run `tmux` and then install the plugin list by hitting `ctrl-a + I` (capital 'I' for 'Install')

## Tmux cheatsheet

The examples below all begin with the `prefix` key, which in my case is `ctrl-a`.
```
ctrl-a + <some option>
```

### Panes
```
%    vert split
"    horz split
o    next
;    previous
z    zoom
q    show numbers
x    kill
{    move left
}    move right
C-o  swap panes
```

### Windows (tabs)
```
c    create
w    list
n    next
p    previous
&    kill
```

### Misc
```
d    detach
t    clock
```

### Plugins
```
tmux-ressurrect
C-s  save
C-r  restore 

tmux-plugin-manager
I    install new plugins / refresh env
U    update plugins
A-u  uninstall plugins
```
