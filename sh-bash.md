- wh
  - whatis apropos info
  - whereis locate
  - which
  - whoami
  - whois
---
---
## api/cli
- env
  - export clear source/`.` exit history printenv set
- file/dir
  - [CRUD]
    - cp mv rm touch ln
    - cat find head tail more less
    - ls cd mkdir pwd
    - diff
  - [meta]
    - chmod chown file stat
  - [zip]
    - gzcat gzip gunzip
  - [printer]
    - lpq lpr lprm
- text
  - echo fmt 
  - [str]
    - awk sed tr wc cut
    - grep egrep fgrep 
  - [row]
    - nl sort uniq
  - nano vi emacs
- process
  - ps top
  - kill killall & nohup
  - sudo
- network
  - dig whois ping wget curl route traceroute host
  - ifconfig netstat lsof
  - scp ssh sftp
- system
  - [job]
    - bg fg jobs 
    - crontab
  - [user]
    - finger last passwd w whoami su
  - [disk]
    - du df quota mount
  - [info]
    - cal date
    - uname uptime pagesize arch
    - man
    - sar ipcs iostat
  - [software-package]
- special
  - sudo trap xargs alias set screen
- develop
  - make 
- help
  - man type help info whatis 
- misc
  - comm paste join tee
  - rsync
  - patch diffstat
  - split
### man
- category
## bash/script
### var
- [crud]
  - name="value"  ((no-sapce))
  - $name ${name}
  - ${#length} ${slice:1:2}
- [literal-type][str][array]
  - 'plain-$text;no-escape' 
  - "expand-$text;allow-escape\n"
  - \`cmd\`
### flow
- [branch]
  - if expr; then stmts; elif expr; stmts; else stmts; fi
  - case expr in; val1 ) stmts; ;; * ) stmts; esac
- [loop]
  - for name in val1 val2 valn; do stmts; done
  - for (( expr1; expr2; expr3 )); do stmts; done
  - while expr; do stmts; done
  - until expr; do stmts; done
  - `while :` `while true` `for (( ; ; ))`
### func
### config
- #!shebang ~/.bashrc ~/.bash_profile
### debug/cli
### shortcut/shell/tui
#### keyboard
### trick
### builtins
### pipe


---
---
---
### reference/guide
- [Idnan/bash-guide: A guide to learn bash](https://github.com/Idnan/bash-guide)
  - [vuuihc/bash-guide: bash 基本用法指南](https://github.com/vuuihc/bash-guide)
- [Learn bash in Y Minutes: Scenic Programming Language Tours](https://learnxinyminutes.com/docs/zh-cn/bash-cn/)
- [fullstack-tutorial/Linux.md at master · frank-lam/fullstack-tutorial](https://github.com/frank-lam/fullstack-tutorial/blob/master/notes/Linux.md)
- [Linux命令搜索引擎](https://wangchujiang.com/linux-command/)
- [Linux命令大全(手册) – Linux命令在线查询网站](https://www.linuxcool.com/)
- [Linux工具快速教程 — Linux Tools Quick Tutorial](https://linuxtools-rst.readthedocs.io/zh_CN/latest/)
### tutorial
- [TLCL](http://billie66.github.io/TLCL/book/) [](#详细的双语混排教材顺便练习英语但不适合速成)
- [30min_guides/shell.md at master · qinjx/30min_guides](https://github.com/qinjx/30min_guides/blob/master/shell.md)
- [the-art-of-command-line/README-zh.md at master · jlevy/the-art-of-command-line](https://github.com/jlevy/the-art-of-command-line/blob/master/README-zh.md)
- [Shell 工具和脚本 · the missing semester of your cs education](https://missing-semester-cn.github.io/2020/shell-tools/)
### EN
- [explainshell.com - match command-line arguments to their help text](https://explainshell.com/)
- [Linux Shell Scripting Tutorial - Bash Linux Shell Scripting Wiki](https://bash.cyberciti.biz/guide/Main_Page)
- [tldr | simplified, community driven man pages](https://tldr.ostera.io/)
- [BashGuide - Greg's Wiki](http://mywiki.wooledge.org/BashGuide)
- [Crontab.guru - The cron schedule expression editor](https://crontab.guru/)
- [Unix - What is Shells?](https://www.tutorialspoint.com/unix/unix-shell.htm)
- [Advanced Bash-Scripting Guide](https://tldp.org/LDP/abs/html/)

