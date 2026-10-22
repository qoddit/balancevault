# TUI and Input

The terminal UI is centered on [[ui.c]] / [[ui.h]] and compatibility helpers in [[curses_compat.h]]. Command parsing and dispatch connect through [[commands.c]].

## Intended interaction model
- Commands are explicitly prefixed with `?`; `-h` displays help.
- Keep permanent key-hint clutter low; reserve space for critical controls.
- Chat name appears in the prompt.
- Scrolling should support keyboard and mouse wheel/trackpad where the terminal emulator emits usable mouse events.

