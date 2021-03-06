# dottmux

My personal `.tmux.conf` settings. Contains custom bindings and plugins.

## Installation

Clone the repo and create a symbolic link to the `.tmux.conf` config file.

```bash
git clone --recursive https://github.com/steven-nichols/dottmux.git ~/.tmux
ln -s ~/.tmux/.tmux.conf ~/.tmux.conf
```

That's it. Enjoy!

## Troubleshooting

First, try reloading the config file:

```bash
tmux source ~/.tmux.conf
```

If the plugins aren't working correctly, double-check that the `--recursive` option was used in the `git clone` command. If not you may need to run this command to fetch the plugins:

```bash
git submodule update --init --recursive
```

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
d    detach (restore by running 'tmux attach')
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
