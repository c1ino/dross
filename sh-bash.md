- wh
  - whatis apropos info
  - whereis locate
  - which
  - whoami
  - whois
---
---
## api/cli
- [env]
  - export clear source/`.` exit history printenv set
- [file/dir]
  - [CRUD]
    - cp mv rm touch ln
    - cat find head tail more less
    - ls cd mkdir pwd rmdir
    - diff
  - [meta]
    - chmod chown file stat
  - [zip]
    - gzcat gzip gunzip
  - [printer]
    - lpq lpr lprm
- [text]
  - echo fmt 
  - [str]
    - awk sed tr wc cut
    - grep egrep fgrep 
  - [row]
    - nl sort uniq
  - nano vi emacs
- [process]
  - ps top
  - kill killall & nohup
  - sudo
- [network]
  - dig whois ping wget curl route traceroute host
  - ifconfig netstat lsof
  - scp ssh sftp
- [system]
  - [job]
    - bg fg jobs 
    - crontab
  - [user]
    - finger last passwd w whoami su
  - [disk]
    - du df quota mount umount
  - [info]
    - cal date
    - uname uptime pagesize arch
    - man
    - sar ipcs iostat
  - [software-package]
- [special]
  - sudo trap xargs alias set screen
- [develop]
  - make 
- [help]
  - man type help info whatis 
- [misc]
  - comm paste join tee
  - rsync
  - patch diffstat
  - split
### man
- category: 1-9
- section
  - NAME, 
    概述(SYNOPSIS), 
    配置(CONFIGURATION), 
    描述(DESCRIPTION), 
    选项(OPTIONS), 
    退出状态(EXIT STATUS), 
    返回值(RETURN VALUE), 
    错误(ERRORS), 
    环境(ENVIRONMENT), 
    文件(FILES), 
    版本(VERSIONS), 
    符合标准(CONFORMING TO), 
    注(NOTES), 
    缺陷(BUGS), 
    示例(EXAMPLE), 
    作者(AUTHORS), 和 
    亦见(SEE ALSO).
## bash/script
### var
- [crud]
  - name="value"  #no-sapce
  - `$name` `${name}`
  - `${#length}` `${slice:start:length}` `${src/pattern/replace}`
- [literal-type]
  - [str]
    - 'plain-$text; no-escape' 
    - "expand-$text; allow-escape\n"
    - \`cmd-output\`
  - [int]
  - [array/hash]
- [special]
### flow
- [branch]
  - if expr; then stmts; elif expr; stmts; else stmts; fi
  - case expr in; val1) stmts;; *) stmts; esac
- [loop]
  - for name in val1 val2 valn; do stmts; done
  - for ((start; end; step)); do stmts; done
  - while expr; do stmts; done
  - until expr; do stmts; done
  - `while :` `while true` `for (( ; ; ))`
### func
### config
- #!shebang ~/.bashrc ~/.bash_profile
### debug/cli
### shortcut/shell/tui
#### keyboard
- ^D
- ^C
### trick
### builtins/cmd
### pipe
### namespace
- alias
- path
- builtins
- function
### section | Debian-manpages
- [shell 内建命令(SHELL BUILTIN COMMANDS)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#shell_内建命令(SHELL_BUILTIN_COMMANDS))
- [历史(HISTORY)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#历史(HISTORY))
- [readline]
  - [Readline Command Names](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#Readline_Command_Names)
  - [readline库(READLINE)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#readline库(READLINE))
    - [Readline Key Bindings](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#Readline_Key_Bindings)
  - [Completing 补全](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#Completing_补全)
    - [Programmable Completion 可编程补全](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#Programmable_Completion_可编程补全)
- [作业控制("JOB CONTROL")](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#作业控制("JOB_CONTROL"))
- [信号(SIGNALS)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#信号(SIGNALS))
- [parse]
  - [命令执行(COMMAND EXECUTION)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#命令执行(COMMAND_EXECUTION))
  - [简单命令扩展("SIMPLE COMMAND EXPANSION")](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#简单命令扩展("SIMPLE_COMMAND_EXPANSION"))
  - [别名(ALIASES)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#别名(ALIASES))
  - [函数(FUNCTIONS)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#函数(FUNCTIONS))
- [重定向(REDIRECTION)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#重定向(REDIRECTION))
- [扩展(EXPANSION)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#扩展(EXPANSION))
  - [Parameter Expansion](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#Parameter_Expansion)
- [Compound Commands 复合命令](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#Compound_Commands_复合命令)
- [保留字("RESERVED WORDS")](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#保留字("RESERVED_WORDS"))
  - [定义(DEFINITIONS)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#定义(DEFINITIONS))
- [启动(INVOCATION)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#启动(INVOCATION))
  - [文件(FILES)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#文件(FILES))
  - [命令执行环境(COMMAND EXECUTION ENVIRONMENT)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#命令执行环境(COMMAND_EXECUTION_ENVIRONMENT))
  - [环境(ENVIRONMENT)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#环境(ENVIRONMENT))
- [cli]
  - [选项(OPTIONS)](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html#选项(OPTIONS))

### tree/toc
- options/cli arguments
- invocation/init
- definitions reserved grammar
  - simple pipelines lists compound comment quoting parameters varaiables arrays
  - expansion substitution
- redirection/io/fd
- alias function 
- evaluation expression expansion
- execution environment exit signals job
- prompting
- readline completing
- history designator
- builtins
- restricted
- files/config



---
---
---
### reference/guide
- [Idnan/bash-guide: A guide to learn bash](https://github.com/Idnan/bash-guide)
  - [vuuihc/bash-guide: bash 基本用法指南](https://github.com/vuuihc/bash-guide)
- [Learn bash in Y Minutes: Scenic Programming Language Tours](https://learnxinyminutes.com/docs/zh-cn/bash-cn/)
- [fullstack-tutorial/Linux.md at master · frank-lam/fullstack-tutorial](https://github.com/frank-lam/fullstack-tutorial/blob/master/notes/Linux.md)
- [Linux命令搜索引擎](https://wangchujiang.com/linux-command/)
- [Linux工具快速教程 — Linux Tools Quick Tutorial](https://linuxtools-rst.readthedocs.io/zh_CN/latest/)
- [Linux命令大全(手册) – Linux命令在线查询网站](https://www.linuxcool.com/)
- [Ubuntu Manpage: man - 系统参考手册的接口](https://manpages.ubuntu.com/manpages/kinetic/zh_CN/man1/man.1.html)
  - [Ubuntu Manpage: Directory Listing](https://manpages.ubuntu.com/manpages/bionic/zh_CN/man1/)
- [模板:Unix命令 - 维基百科](https://zh.wikipedia.org/wiki/Template:Unix命令)
  - [Unix实用程序列表 - 维基百科](https://zh.wikipedia.org/wiki/Unix实用程序列表)
- [bash(1) — manpages-zh — Debian bullseye — Debian Manpages](https://manpages.debian.org/testing/manpages-zh/bash.1.zh_CN.html)
  - [man(1) — man-db — Debian testing — Debian Manpages](https://manpages.debian.org/testing/man-db/man.1.zh_CN.html)
  - [intro(1) — manpages-zh — Debian bullseye — Debian Manpages](https://manpages.debian.org/testing/manpages-zh/intro.1.zh_CN.html)

### tutorial
- [Shell 工具和脚本 · the missing semester of your cs education](https://missing-semester-cn.github.io/2020/shell-tools/)
- [Shell 教程 | 菜鸟教程](https://www.runoob.com/linux/linux-shell.html)
  - [30min_guides/shell.md at master · qinjx/30min_guides](https://github.com/qinjx/30min_guides/blob/master/shell.md)
- [TLCL](https://billie66.github.io/TLCL/book/) [](#详细的双语混排教材顺便练习英语但不适合速成)
- [the-art-of-command-line/README-zh.md at master · jlevy/the-art-of-command-line](https://github.com/jlevy/the-art-of-command-line/blob/master/README-zh.md)
- [Shell编程基础 - Ubuntu中文](https://wiki.ubuntu.org.cn/Shell编程基础)
- [网络、文本处理工具与 Shell 脚本 - Linux 101](https://101.lug.ustc.edu.cn/Ch06/)
- [学习Linux — 学习Linux](https://linux.fasionchan.com/zh_CN/latest/index.html)

### EN
- [GNU Bash manual - GNU Project - Free Software Foundation](https://www.gnu.org/software/bash/manual/)
- [explainshell.com - match command-line arguments to their help text](https://explainshell.com/)
- [Linux Shell Scripting Tutorial - Bash Linux Shell Scripting Wiki](https://bash.cyberciti.biz/guide/Main_Page)
- [tldr | simplified, community driven man pages](https://tldr.ostera.io/)
- [BashGuide - Greg's Wiki](https://mywiki.wooledge.org/BashGuide)
- [Crontab.guru - The cron schedule expression editor](https://crontab.guru/)
- [Unix - What is Shells?](https://www.tutorialspoint.com/unix/unix-shell.htm)
- [Advanced Bash-Scripting Guide](https://tldp.org/LDP/abs/html/)
- [Ubuntu Manpage: Welcome](https://manpages.ubuntu.com/)
- [man page - Wikipedia](https://en.wikipedia.org/wiki/Man_page)
  - [Template:Unix commands - Wikipedia](https://en.wikipedia.org/wiki/Template:Unix_commands)
- [index — Debian Manpages](https://manpages.debian.org/)
- [Linux Man Page Howto](https://tldp.org/HOWTO/Man-Page/)

