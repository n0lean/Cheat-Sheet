# Tmux Cheat Sheet

## Most used

```bash
tmux at # reconnect to a session
tmux ls # = tmux list-session
tmux kill-server # close all session
```

```
C-b : # enter command line
C-b d # detach
C-b [0-9] # enter window [0-9]
C-b , # rename window
C-b & # close window
C-b c # new window
```

## Command

1. Info

```bash
tmux list-keys
tmux list-commands
tmux info
```

2. Session

```bash
tmux new -s session_name
tmux attach -t session_name
tmux switch -t session_name
tmux detach
```

3. Window

```bash
tmux new-window
tmux list-windows
tmux select-window -t :0-9
tmux rename-window
```

4. Pane

```bash
tmux split-window
tmux split-window -h # honrizontal
tmux swap-pane -[UDLR] # Switch panes in [UDLR] direction
```

## Hotkeys

First C-b, then:

1. General

| keys | command               |
| ---- | --------------------- |
| ?    | help                  |
| d    | detach                |
| s    | switch session        |
| D    | detach target session |
| :    | command line mode     |
| [    | copy mode             |
| ]    | paste mode            |
| t    | show time             |
| ~    | show logs             |

2. Window

| keys  | command                         |
| ----- | ------------------------------- |
| c     | new window                      |
| &     | close                           |
| [0-9] | switch to [0-9]                 |
| l     | switch to previous              |
| ,     | rename                          |
| .     | reorder                         |
| f     | search keywords in window names |

3. Pane

| keys                         | command                |
| ---------------------------- | ---------------------- |
| "                            | split vertically       |
| %                            | split horizontally     |
| [UDLR]                       | focus to [UDLR]        |
| ctrl + [UDLR] / alt + [UDLR] | change pane size       |
| x                            | close                  |
| z                            | maximize current panel |