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
- Messages ((消息/事件))
### SystemTiddlers
/ [SystemTiddlers | TiddlyWiki](<https://tiddlywiki.com/#SystemTiddlers>)

- DefaultTiddlers
- Keyboard Shortcut Tiddler
- $:/info/
- $:/config/
- $:/plugins/
- $:/core/
- [misc]
  - $:/tags/
  - $:/language/
  - $:/theme/
  - $:/StoryList 
  - $:/HistoryList
- [Naming of System Tiddlers | TiddlyWiki](<https://tiddlywiki.com/#Naming of System Tiddlers>)
#### Plugins
- :plugin-type
  - plugin theme language import info
- /plugin.info
##### misc
- [Developing plugins using Node.js and GitHub | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Developing plugins using Node.js and GitHub>)
- $:/core
- railroad
### Modules 
/ [Modules | TiddlyWiki](https://tiddlywiki.com/#Modules)

- module-type / [ModuleType | TiddlyWiki](https://tiddlywiki.com/#ModuleType)
- Macro.exports
  - name: macro_name
  - params: [list]
    - name: param_name
    - default
  - run: func 
- Widget.exports
  - [:widget_name] = factory()
    - prototype = new require("$:/core/modules/widgets/widget.js").widget()
      - render() refresh()  
####
- [JavaScript Macros | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/index.html#JavaScript Macros>)
- [TiddlyWiki5/core/modules/macros at master · Jermolene/TiddlyWiki5](https://github.com/Jermolene/TiddlyWiki5/tree/master/core/modules/macros)
- [Module System | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Module System>)

### Messages
/ [Messages | TiddlyWiki/Dev](https://tiddlywiki.com/dev/#Messages)

- :name, :parameter
- ActionWidgets, TriggeringWidgets 
  - `<$action-sendmessage ...>`
- MessageHandlerWidgets

## tree
- WikiText
  - Widget
    - Macro
    - Variable
    - Message
    - Module
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
## data-struct
- [Data Storage in Single File TiddlyWiki | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Data Storage in Single File TiddlyWiki>)
- [Datamodel | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Datamodel>)
- [TiddlyWiki Architecture | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#TiddlyWiki Architecture>)
