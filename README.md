# Searchable popup of sway/i3 keybindings.

Reads the live config via `swaymsg -t get_config` (or i3-msg), which keeps
comments and resolves includes, then shows the bindings in rofi.

Descriptions come from, in order of preference:
  1. the comment line(s) immediately above a run of bindsym lines
  2. a tidied-up version of the command itself

Selecting an entry runs that binding's command.
