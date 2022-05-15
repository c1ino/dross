
# idlelib
- cli
  - -r (run)
  - -e (editor)
  - -d (debugger)
  - -t (title)
  - \- (stdin)
  - (startup)
    - IDLESTARTUP, PYTHONSTARTUP
  - (workaround)
- config
  - ~/.idlerc
- menu-bar
  - file
  - edit
  - shell
  - debug
  - options
  - window
  - help
- editor
- shell
  - debugger
    - stack-viewer
  - history
    - ^prev/next, return
- ctx-menu
  - Squeezed text
    - view in new win
  - jump to exception
## key bindings/shortcuts/hotkeys/key-set
>https://docs.python.org/zh-cn/3/library/idle.html#key-bindings
- system
- tcl/tk
  - (navigate)
    - ^a, ^e = ahead, end
    - ^f, ^b = forward/left, backward/right
    - ^p, ^n = prev/up, next/down
    - ^i
  - (edit)
    - ^d, ^k = del-next-char, del-to-end-of-line/kill-line
- idlelib
  - #, = preferences
  - (edit)
    - (navigate)
      - #j = jumpto-line
    - (move)
      - #\[, #\] = indent
    - (hint)
      - ^0 = flash-paren
      - ^\ = call-tip
      - !/ = expand
      - ^space = completions
    - (edit)
      - #c, #x, #v
      - (comment, undo/redo, find/replace)
  - (execute)
    - ^c = interrupt
    - ^d = eof
    - ^F6 = restart-shell
  - (window)
    - #n/w = new/close-window
    - #m, #b


[console manual page - Tk Built-In Commands]:(https://www.tcl.tk/man/tcl8.7/TkCmd/console.html#M13)
