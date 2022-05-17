# pdb
- set_trace()
  - breakpoint() (3.7+)
- pm()
  - post_mortem(:traceback)
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
  - h/help :cmd
    - pdb, !/exec
  - (repeat-last-cmd)
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
  - s/step  ((step-into-stack))
    - n/next  ((next-line))
    - r/return ((return-to-previous-frame))
  - unt/unill :lineno
  - c/continue
  - j/jump :lineno
- (inspect)
  - l/list, ll/longlist
  - a/args
  - p :expr
    - pp
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
  - (completekey='tab', stdin=None, stdout=None, skip=None, nosigint=False, readrc=True)
