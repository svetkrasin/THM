# Launch a new session

tmux

# How to use

all tmux commands start with combination 

ctrl + b

then release the combination,
and press the following key-command

<ctrl + b> + cs

lets call <ctrl + b> - <prefix>

# Detach from the session

<prefix> + d

# List all sessions

tmux ls

# Attatch to a session

tmux a -t <session>

# Make a new window

<prefix> + c

# Enter the copy mode

<prefix> + [

# Exit the copy mode

q

# Split the window vertically

%

# Split the window horizontally

"

# Navigate between panes

<prefix> + <arrow keys>

# Kill a pane

<prefix> + x

# Close the session

exit

# Spawn a named session

tmux new -s <name>
