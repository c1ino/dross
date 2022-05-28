- regular-expr
  - r'real-str'
  - special-char `.^$*+?{}\[]|()`
  - flags
- re
  - compile(:pat, :flags) -> Pattern
    - .flags, .groups, .groupindex, .pattern
  - (operation)
    - split(..., :maxsplit, \*)
    - findall/finditer(..., \*)
    - sub/subn(:pat, :repl, :str, :count, \*)
  - search/match/fullmatch(:pat, :str, :flags) -> Match
    - .pos, .endpos, .lastindex, .lastgroup, .re, .string
    - expand(:repl)
    - group(:gindex, ...)\
      [:gindex]\
      groups(:fallback)\
      groupdict(:fallback)
    - start/end/span(:gindex)
  - (auxiliary) 
    - escape(:pat)
    - purge()
- regular-expr
  - :repl `\g1` `\g<1>` `\g<name>`
    - `\g0` self
