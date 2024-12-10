# Tmux Cheat Sheet

# Sessions

### Start a new session
- **Description**: Start a new session.
- **Keywords**: create
- **Shell**:
  - `tmux`
  - `tmux new`
  - `tmux new-session`
- **Tmux Command**: `new`

---

### Start or attach to a session named *mysession*
- **Description**: Start a new session or attach to an existing session named *mysession*.
- **Keywords**: create, attach, join
- **Shell**:
  - `tmux new-session -A -s mysession`

---

### Start a session with the name *mysession*
- **Description**: Start a new session with the name *mysession*.
- **Keywords**: create
- **Shell**:
  - `tmux new -s mysession`
- **Tmux Command**: `new -s mysession`

---

### Kill/delete the current session
- **Description**: Terminate the current session.
- **Keywords**: terminate
- **Tmux Command**: `kill-session`

---

### Kill/delete session *mysession*
- **Description**: Terminate a session named *mysession*.
- **Keywords**: terminate
- **Shell**:
  - `tmux kill-ses -t mysession`
  - `tmux kill-session -t mysession`

---

### Kill/delete all sessions but the current
- **Description**: Terminate all sessions except the current one.
- **Keywords**: terminate
- **Shell**: `tmux kill-session -a`

---

### Rename session
- **Description**: Rename the current session.
- **Shortcut**: `Ctrl + b $`

---

### Detach from session
- **Description**: Exit the current session.
- **Keywords**: exit session
- **Shortcut**: `Ctrl + b d`

---

### Detach others on the session
- **Description**: Detach other clients in the current session to maximize the window.
- **Keywords**: exit session, detach others, maximize
- **Tmux Command**: `attach -d`

---

### Show all sessions
- **Description**: List all active sessions.
- **Shell**:
  - `tmux ls`
  - `tmux list-sessions`
- **Shortcut**: `Ctrl + b s`

---

### Attach to the last session
- **Description**: Attach to the most recent session.
- **Shell**:
  - `tmux a`
  - `tmux at`
  - `tmux attach`
  - `tmux attach-session`

---

### Attach to a session named *mysession*
- **Description**: Attach to a session with the name *mysession*.
- **Shell**:
  - `tmux a -t mysession`
  - `tmux at -t mysession`
  - `tmux attach -t mysession`
  - `tmux attach-session -t mysession`

---

### Session and Window Preview
- **Description**: Preview available sessions and windows.
- **Keywords**: navigate, switch
- **Shortcut**: `Ctrl + b w`

---

### Move to previous session
- **Description**: Navigate to the previous session.
- **Keywords**: navigate, switch
- **Shortcut**: `Ctrl + b (`

---

### Move to next session
- **Description**: Navigate to the next session.
- **Keywords**: navigate, switch
- **Shortcut**: `Ctrl + b )`

---

# Windows

### Start a session with a specific window
- **Description**: Start a new session named *mysession* with a window named *mywindow*.
- **Keywords**: create
- **Shell**: `tmux new -s mysession -n mywindow`

---

### Create a new window
- **Description**: Create a new window in the current session.
- **Keywords**: create new window
- **Shortcut**: `Ctrl + b c`

---

### Rename the current window
- **Description**: Rename the active window.
- **Shortcut**: `Ctrl + b ,`

---

### Close the current window
- **Description**: Kill/delete the active window.
- **Keywords**: kill window, delete window
- **Shortcut**: `Ctrl + b &`

---

### List windows
- **Description**: Display all windows in the current session.
- **Keywords**: list window, show window
- **Shortcut**: `Ctrl + b w`

---

### Toggle last active window
- **Description**: Switch to the last active window.
- **Shortcut**: `Ctrl + b l`

---

# Panes

### Split the current pane horizontally
- **Description**: Split the pane with a vertical line to create a horizontal layout.
- **Tmux Command**: `split-window -h`
- **Shortcut**: `Ctrl + b %`

---

### Split the current pane vertically
- **Description**: Split the pane with a horizontal line to create a vertical layout.
- **Tmux Command**: `split-window -v`
- **Shortcut**: `Ctrl + b "`

---

### Toggle synchronize-panes
- **Description**: Send commands to all panes simultaneously.
- **Tmux Command**: `setw synchronize-panes`

---

### Toggle between pane layouts
- **Description**: Cycle through available pane layouts.
- **Shortcut**: `Ctrl + b Spacebar`

---

## Panes

- **Switch to next pane**
  - **Shortcut:** `Ctrl` + `b` `o`

- **Show pane numbers**
  - **Shortcut:** `Ctrl` + `b` `q`

- **Switch/select pane by number**
  - **Shortcut:** `Ctrl` + `b` `q` `0` ... `9`

- **Toggle pane zoom**
  - **Shortcut:** `Ctrl` + `b` `z`

- **Convert pane into a window**
  - **Shortcut:** `Ctrl` + `b` `!`

- **Resize current pane height (holding second key is optional)**
  - **Shortcut:**
    - `Ctrl` + `b` + ↑
    - `Ctrl` + `b` `Ctrl` + ↑
    - `Ctrl` + `b` + ↓
    - `Ctrl` + `b` `Ctrl` + ↓

- **Resize current pane width (holding second key is optional)**
  - **Shortcut:**
    - `Ctrl` + `b` + →
    - `Ctrl` + `b` `Ctrl` + →
    - `Ctrl` + `b` + ←
    - `Ctrl` + `b` `Ctrl` + ←

- **Close current pane**
  - **Shortcut:** `Ctrl` + `b` `x`

## Copy Mode

- **Use vi keys in buffer**
  - **Command:** `setw -g mode-keys vi`

- **Enter copy mode**
  - **Shortcut:** `Ctrl` + `b` `[`

- **Enter copy mode and scroll one page up**
  - **Shortcut:** `Ctrl` + `b` `PgUp`

- **Quit mode**
  - **Shortcut:** `q`

- **Go to top line**
  - **Shortcut:** `g`

- **Go to bottom line**
  - **Shortcut:** `G`

- **Scroll up**
  - **Shortcut:** ↑

- **Scroll down**
  - **Shortcut:** ↓

- **Move cursor left**
  - **Shortcut:** `h`

- **Move cursor down**
  - **Shortcut:** `j`

- **Move cursor up**
  - **Shortcut:** `k`

- **Move cursor right**
  - **Shortcut:** `l`

- **Move cursor forward one word at a time**
  - **Shortcut:** `w`

- **Move cursor backward one word at a time**
  - **Shortcut:** `b`

- **Search forward**
  - **Shortcut:** `/`

- **Search backward**
  - **Shortcut:** `?`

- **Next keyword occurrence**
  - **Shortcut:** `n`

- **Previous keyword occurrence**
  - **Shortcut:** `N`

- **Start selection**
  - **Shortcut:** `Spacebar`

- **Clear selection**
  - **Shortcut:** `Esc`

- **Copy selection**
  - **Shortcut:** `Enter`

- **Paste contents of buffer_0**
  - **Shortcut:** `Ctrl` + `b` `]`

- **Display buffer_0 contents**
  - **Command:** `show-buffer`

- **Copy entire visible contents of pane to a buffer**
  - **Command:** `capture-pane`

- **Show all buffers**
  - **Command:** `list-buffers`

- **Show all buffers and paste selected**
  - **Command:** `choose-buffer`

- **Save buffer contents to buf.txt**
  - **Command:** `save-buffer buf.txt`

- **Delete buffer_1**
  - **Command:** `delete-buffer -b 1`

## Misc

- **Enter command mode**
  - **Shortcut:** `Ctrl` + `b` `:`

- **Set OPTION for all sessions**
  - **Command:** `set -g OPTION`

- **Set OPTION for all windows**
  - **Command:** `setw -g OPTION`

- **Enable mouse mode**
  - **Command:** `set mouse on`

## Help

- **List key bindings (shortcuts)**
  - **Shortcut:** `Ctrl` + `b` `?`
  - **Command:** `tmux list-keys`

- **Show every session, window, pane, etc.**
  - **Command:** `tmux info`

