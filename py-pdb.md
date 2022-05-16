# pdb
- set_trace/breakpoint
- pm/post_mortem
- run(:stmt)
  - eval, call

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
  - alias :name :cmd %* %1
    - unalias
- (stack)
  - w/where
  - d/down, u/up
- (breakpoint)
  - b/break :lineno/func
  - tbreak  ((tempbreak))
  - cl/clear
  - disable, enable, ignore
  - condition
  - commands
- (execute)
  - s/step  ((step-into))
    - n/next  ((next-line))
  - unt/unill :lineno
  - r/return
  - c/continue
  - j/jump :lineno
- (inspect)
  - l/list, ll/longlist
  - a/args
  - p :expr, pp
  - whatis :expr  ((type-of-expr))
  - source :expr 
  - display :expr 
    - undisplay
  - retval  ((func-last-return-value))
- (debug)
  - interact  ((interactive-shell))
  - debug :stmt  ((pdb.run(:stmt)))
- (process)
  - run :args
    - restart
  - q/quit


## class
- Pdb
