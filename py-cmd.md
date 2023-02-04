

## Cmd
- [init]
  - cmd.Cmd(completekey='tab', stdin=None, stdout=None)  
- [main]
  - cmdloop(intro=None)
  - onecmd(str)
  - emptyline()
  - default(line)
  - completedefault(text, line, begidx, endidx)
- [hook]
  - precmd postcmd preloop postloop
- [shell]
  - `do_*`
  - `?` `do_help` `help_*`
  - `!` `do_shell`
- [attr]
  - prompt \
    intro
  - cmdqueue lastcmd  
  - ruler doc_header misc_header undoc_header
  - use_rawinput
  - identchars
