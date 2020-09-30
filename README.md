# Linux tips and tricks

## Table of content

[Toc]





## NERDTree

Installation https://github.com/preservim/nerdtree

Usage:

* Move between windows: `Ctrl` + `w` then `w`
* 

## Practical tmux
Similar to `screen`, but more userfriendly, great to work in bash interactive mode, exit (detach), then return to it later (attach).

- Start a tmux session
`$tmux`(default name from `0`)
or
`$tmax new -s <session_name>`


- Split screen (within tmux): press `Ctrl+b` then `%`
- Move between screens: `Ctrl+b` then &larr; or &rarr; 
- Detach the current session: `Ctrl+b` then `d`

- Views the detached sessions (outside of tmux)
`$tmux ls`

- Attach to a detached session:
`$tmux attach -t <session_name>`

- Kill a tetached session
`$tmux kill-session -t <session_name>`

## LaTeX stuffs

### Styled block quotes

```latex
\usepackage[strict]{changepage}
\usepackage{framed}
\usepackage{etoolbox}
\AtBeginEnvironment{quote}{
   \def\FrameCommand{
       {\color{lightgray}\vrule width 4pt}
       \color{gray}
   }
   \MakeFramed{}  
}
\AtEndEnvironment{quote}{\endMakeFramed}
```




