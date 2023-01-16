## Reference
- WikiText
- Filters
  - `[operator[parameter]]`  
- Macros
  - `\define name(param) \end`
  - `<<name arg>>`
- Variables
  - `<<var>>`
  - `$var$` `$(var)$` `<<var>>` `<<__var__>>`
- Widgets
  - `<$name para=arg> slot </name>`
  - `<$name para=arg/>`
- Messages
- [misc]
  - Commands
  - Mechanisms
## Concept
- Tiddlers ((条目))
  - TiddlerFields ((字段))
  - Tagging ((标签))
  - SystemTiddlers ((系统条目))
  - ShadowTiddlers ((影子条目))
  - DataTiddlers ((数据条目))
  - (TemplateTiddlers) ((模板条目))
- Modules ((模块))
  - (*.js)
- Plugins ((插件))
  - `$:/plugins/publisher/name`
- Pragma ((编译指示))
- WikiText
  - Transclusion ((嵌入))
    - `{{tiddler!!field}}`
    - `{{tiddler||template_tiddler}}`
  - Substitution ((替换))
    - (Macro, Variable)
  - Typed Blocks 
  - Links
  - CSS
- TextReference
### SystemTiddlers
- DefaultTiddlers
- Keyboard Shortcut Tiddler
#### Plugins
- $:/core
- railroad
### Modules 
/ [JavaScript Macros | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/index.html#JavaScript Macros>)

- exports
  - name: macro_name
  - params: [list]
    - name: param_name
    - default
  - run: func 

[TiddlyWiki5/core/modules/macros at master · Jermolene/TiddlyWiki5](https://github.com/Jermolene/TiddlyWiki5/tree/master/core/modules/macros)

## tree
- WikiText
  - Widget
    - Macro
      - Module
    - Message
    - Variable
  - TextReference
  - Filter
    - [Title List]
- Tiddler
  - Tiddler Fields
    - Tagging
  - [type]
    - System Tiddler
      - Plugin
        - Shadow Tiddler
    - Data Tiddler
    - Module Tiddler
    - (Template Tiddler)
