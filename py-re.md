- regular-expr
  - r'real-str'
  - special-char `.^$*+?{}\[]|()`
  - flags
- re
  - compile(:pat, :flags) -> Pattern
    - flags, groups, groupindex, pattern
  - search/match/fullmatch(:pat, :str, :flags) -> Match
    - expand()
      group()
      [:group-index]
      groups()
      groupdict()
      start/end/span()
    - pos, endpos, lastindex, lastgroup, re, string
  - split(..., :maxsplit, \*)
  - findall/finditer(..., \*)
  - sub/subn(:pat, :repl, :str, :count, \*)
  - (auxiliary) 
    - escape(:pat)
    - purge()
