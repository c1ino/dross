- regular-expr
  - r'real-str'
  - special-char `.^$*+?{}\[]|()`
  - flags
- re
  - compile(:pat, :flags) -> Pattern
    - flags, groups, groupindex, pattern
  - Match
    - expand()
      group()
      [:group-index]
      groups()
      groupdict()
      start/end/span()
    - pos, endpos, lastindex, lastgroup, re, string
  - search()
    match()
    fullmatch()
    split()
    findall()
    finditer()
    sub()
    subn()
    escape()
    purge()
