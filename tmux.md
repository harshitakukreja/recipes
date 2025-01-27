# Create a new session
```bash
tmux new -s <session_name>
```

# Detach from a session
`^B` then `D`

# Attach to a session
```bash
tmux a -t <session_name>
```

# List all sessions
```bash
tmux ls
```

# Kill a session 
## From inside the session
`^D`
## From outside the session
```bash
tmux kill-session -t <session_name>
```

# Scroll mode
## Enter
`^B` then `[`
## Exit
`ESC` and wait for a second


