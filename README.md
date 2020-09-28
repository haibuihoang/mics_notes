# mics_notes
Misclaneous notes


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

