

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
  - do_*
  - ? help_* do_help
  - ! do_shell
