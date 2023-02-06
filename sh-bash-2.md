
## toc
- [cli]
  - options arguments
- [init]
  - invocation
- [grammar]
  - definitions reserved 
  - grammar
    - simple pipelines lists compound comment quoting parameters varaiables arrays
  - expansion substitution
    - brace expansion(花括号扩展)
    - tilde expansion(波浪线扩展)
    - parameter and variable expansion(参数和变量扩展)
    - command substitution(命令替换)
    - arithmetic expansion(算术扩展)
    - word splitting(词的拆分)
    - pathname expansion(路径扩展)
    - process subtitution (进程替换)
  - redirection/io/fd
  - alias function 
  - evaluation expression expansion
    - ARITHMETIC EVALUATION
    - CONDITIONAL EXPRESSIONS
    - SIMPLE COMMAND EXPANSION
- execution environment exit signals job
- [tui]
  - prompting
  - readline completing
    - Notation Initialization Key-Bindings Variables Conditional-Constructs Searching 
    - Command-Names
      - Moving History Text Clip Numeric Completing Macros Miscellaneous
    - Programmable-Completion
  - history/designator
    - HISTORY EXPANSION
    - Event Designators
    - Word Designators
    - Modifiers  
- builtins
  - [env]
    - source alias/unalias declare/typeset export
    - getopts local readonly set/unset shift  
    - builtin command enable
  - [job/process]
    - bg fg jobs disown 
    - kill suspend trap wait
  - [readline]
    - bind compgen complete
  - [flow]
    - exit break continue return
  - [tree/dir]
    - cd dirs pushd popd pwd
  - [io/text]
    - echo printf read
  - [history]
    - fc history
  - [system]
    - logout
    - times ulimit umask
  - [misc]
    - eval exec let test
    - help type 
    - hash shopt
- restricted
- [config]
  - files

### Grammar
#### Definitions
- blank
- word ((token))
- name ((identifier))
- metacharacter ((sep))
  - `| & ; ( ) < > space tab` 
- control-operator
  - `|| & && ; ;; ( ) | <newline>`
#### Compound Commands
- [*]
  - (list)
  - { list; }
  - ((expr))
  - [[ expr ]]
- [flow]
  - if case
  - for while until 
  - select
- function name(){list;}
#### Parameters
- positional/arguments
- special/readonly
  - \* @ # ? - $ ! 0
- shell
#### Expansion / Subtitution
- [priority]
  - brace, tilde, parameter, variable, arithmetic, command, splitting, pathname
- Brace Expansion  `{...}`
- Tilde Expansion  `~`
- Parameter Expansion  `$...`
- Command Substitution `$(cmd)` \`cmd\`
- Arithmetic Expansion `$((expr))`
- Process Substitution `<(list)` `>(list)`
- Word Splitting
- Pathname Expansion `*?[`
- Quote Removal `\'"`
#### Evaluation / Expansion
- ARITHMETIC EVALUATION
- CONDITIONAL EXPRESSIONS
- SIMPLE COMMAND EXPANSION
#### (Execution / Environment)
#### (Exit / Signals / Job Control)

### Builtins
####
##### 

## (tree)
- [stmt]
  - simple-commands
  - pipelines
  - lists
  - compound-commands
  - comments
  - quoting
- [parameter]
  - value attributes
  - [set/assign]
  - [get]
  - positional special shell arrays

---
---
---
## section | Debian-manpages
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
