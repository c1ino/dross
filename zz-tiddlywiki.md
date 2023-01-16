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
  - Tagging ((添加标签))
  - SystemTiddlers ((系统条目))
  - ShadowTiddlers ((影子条目))
  - DataTiddlers ((数据条目))
  - (TemplateTiddlers) ((条目模板))
- Modules ((模块))
  - (*.js)
- Plugins ((插件))
  - `$:/plugins/publisher/name`
- Pragma ((编译指令))
- WikiText
  - Transclusion ((嵌入)) (独立渲染)
    - `{{tiddler!!field}}`
    - `{{tiddler||template_tiddler}}`
  - Substitution ((替换)) (预处理)
    - (Macro, Variable)
  - Typed Blocks ((类型区块))
    - `$$$content-type/.ext \n...\n $$$`
  - Links ((链接))
    - Hard (literal)
    - Soft (dynamic-render)
  - Styles and Classes ((样式与类))
    - `@@style:val;/.class \n...\n @@`
- TextReference ((文本引用))
- Filter ((过滤器))
- Messages ((部件消息/事件))
- Macros ((宏))
- Widgets ((部件))
- Variables ((变量))
- Commands ((命令行命令))
- Mechanisms ((机制))
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
- [Developing plugins using Node.js and GitHub | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Developing plugins using Node.js and GitHub>)
##### misc
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

## see-also
- [TiddlyWiki — a non-linear personal web notebook](<https://tiddlywiki.com/>)
- [TiddlyWiki/Dev — documentation for developers](<https://tiddlywiki.com/dev/>)
- [TiddlyWiki 舞 — 基礎文件正體中文版](https://tw5-zh.tiddlyspot.com/)
- [(ver.5.1.15) TiddlyWiki — 非线性个人网络笔记本](https://oss.hintsnet.com/mirror/tiddlywiki.cn.html)
  - [(http) TiddlyWiki — 非线性个人网络笔记本](http://oss.hintsnet.com/mirror/tiddlywiki.cn.html)
- [(http) TiddlyWiki 备忘录 — 官网副本中文版 • 2021年11月1日](http://tiddlywiki.cn/)
