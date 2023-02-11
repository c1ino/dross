## tree1
- [expr]
  - literal
  - variable
  - operator
- [stmt]
  - [flow]
    - [branch / loop / error]
  - method
- [oop]
  - class
  - module
- [misc]
### tree2
- [expr]
  - literal
    - [number] / String / [bool] / nil / Array / Hash
    - Symbol / Proc / [percent]
    - Range / Regexp
  - variable
    - local / ::Const / $global / @instattr / @@clsattr
  - operator
    - assign / calculate / compare / logic / bit / range 
    - [special]
      - defined? / dot`.` / namespace`::` / index`[]`
- [stmt]
  - [flow] / modifier
    - [branch]  
      - if / unless / case-when / [ternary]
    - [loop] 
      - while / until / for-in
        - break / next / redo
    - [error]
      - begin / rescue / ensure 
        - retry / raise
  - [function] method
    - def / [proc] / &block{} / do / lambda
- [oop]
  - class
  - module
  - [mixin] 
    - include / extend / prepend
- [misc]
  - [comment]
  - require / load
  - alias / undef
  - BEGIN / END

## feature
## style / design
