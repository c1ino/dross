# pdb
- set_trace/breakpoint
- pm/post_mortem
- run(:stmt), (eval, call)

## cli
- -c :cmd 
- -m :mod (3.7+)

## config
- ~/.pdbrc

## cmd
- (sugar)
  - !stmt
  - cmd1;; ...
  - help :cmd
    - pdb, !/exec
  - alias :name :cmd %* %1, unalias
- (stack)
  - w/where
  - d/down, u/up
- (breakpoint)
  - b/break :lineno/func
  - tbreak (tempbreak)
  - cl/clear
  - disable, enable, ignore
  - condition
  - commands
- (execute)
  - s/step, n/next
  - unt/unill
  - r/return
  - c/continue
  - j/jump
- (inspect)
  - l/list, ll/longlist
  - a/args
  - p :expr, pp
  - whatis :expr
  - source :expr
  - display :expr, undisplay
  - retval
- (debug)
  - interact (interactive-shell)
  - debug :stmt (sub-pdb-into-stmt)
- (process)
  - run :args, restart
  - q/quit


## class
- Pdb
