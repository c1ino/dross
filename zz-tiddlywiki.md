## Reference
- WikiText
- Filters
  - `[operator[parameter]]`  
    - [full-form] `[operator:suffix[parameter]]`
    - [shortcut] 
      - `[[param]]` `["param"]` `['param']` == `[title[param]]`
      - `[anyfield[param]]` == `[field:anyfield[param]]`
  - [operation]
    - [not] `[!op[param]]`
    - [and-select] `[op1[pa1]op2[pa2]...]`
    - [or-select/union] `[op1[pa1]] [op2[pa2]] ...`
    - [and-pipe/intersection] `[op1[pa1]] ... +[op2[pa2]]`
    - [remove-pipe/subtraction] `[op1[pa1]] ... -[op2[pa2]]`
  - [parameter]
    - [literal/quote] `[op[literal with space]]`
    - [TextReference] `[op{textReference}]`
    - [Varaiable] `[op<var1>]`
- Macros
  - `<<name arg>>`
  - `\define name(param) \n...\n \end`
- Variables
  - `<<var>>`
  - `$var$` `$(var)$` `<<var>>` `<<__var__>>`
- Widgets
  - `<$name para=arg/>`
  - `<$name para=arg> ... </$name>`
- Messages
- [misc]
  - Commands
  - Mechanisms
## Concepts
- Tiddlers ((条目))
  - TiddlerFields ((字段))
  - Tagging ((添加标签))
  - [SystemTiddlers ((系统条目))](#systemtiddlers)
  - ShadowTiddlers ((影子条目))
  - DataTiddlers ((数据条目))
  - (TemplateTiddlers) ((条目模板))
- [Modules ((模块))](#modules)
  - (*.js)
- [Plugins ((插件))](#plugins)
  - `$:/plugins/publisher/name`
- Pragma ((编译指令)) / [Pragma | TiddlyWiki](<https://tiddlywiki.com/languages/zh-Hans/index.html#Pragma>)
  - `\define` `\rules` `\import`
- WikiText
  - Transclusion ((嵌入)) (独立渲染)
    - `{{tiddler!!field}}`
    - `{{tiddler||template_tiddler}}`
    - `{{!!field}}`
    - `{{data_tiddler##index}}`
    - `{{{ [tag[mechanism]] ||template_tiddler}}}`
  - Substitution ((替换)) (预处理)
    - (Macro, Variable)
  - Typed Blocks ((类型区块))
    - `$$$content-type/.ext \n...\n $$$`
  - Links ((链接))
    - Hard (literal-static)
    - Soft (dynamic-render)
  - Styles and Classes ((样式与类))
    - `@@style:val;/.class \n...\n @@`
- TextReference ((文本引用))
- Filters ((过滤器))
  - input (default: [all[tiddlers]])
  - [expression]
    - runs ((运行块))
      - steps ((步骤))
        - prefix `!`
        - operator ((操作符/运算符))
          - selection modifiers（选择修饰符）
          - selection constructors（选择构造器）
        - suffix `:suf`
        - parameter/operand
  - output
    - title selection（标题选集）是一组有序的条目标题（或类似的字符串），其中没有标题会出现一次以上。
- [Messages ((部件消息/事件))](#messages)
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
- [SystemTags | TiddlyWiki](<https://tiddlywiki.com/languages/zh-Hans/index.html#SystemTags>)
### Plugins
/ [PluginMechanism | TiddlyWiki](<https://tiddlywiki.com/#PluginMechanism>)

- :plugin-type
  - plugin theme language import info
- /plugin.info
- [Developing plugins using Node.js and GitHub | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Developing plugins using Node.js and GitHub>)
#### misc
- $:/core
- railroad
### Modules 
/ [Modules | TiddlyWiki](https://tiddlywiki.com/#Modules)

- :module-type / [ModuleType | TiddlyWiki](https://tiddlywiki.com/#ModuleType)
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

### Filters
#### Operators
- Math
  - [map]: unary, binary
  - reduce

## tree
- WikiText
  - Widget
    - Macro
    - Variable
    - Message
    - Module
  - TextReference
  - Filter
    - [Title List] [Title Selection]
  - Pragma
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
- System
  - core config plugins theme language
## data-struct
- [Data Storage in Single File TiddlyWiki | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Data Storage in Single File TiddlyWiki>)
- [Datamodel | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#Datamodel>)
- [TiddlyWiki Architecture | TiddlyWiki/Dev](<https://tiddlywiki.com/dev/#TiddlyWiki Architecture>)

## glossary

|en|Hans|Hant|
|-|-|-|
|widget|部件|小工具|
|message|部件消息/事件|小工具讯息|
|macro|宏|巨集|
|variable|变量|变数|
|filter|过滤器|筛选器|
|data|数据|资料|
|field|字段|栏位|
|link|链接|连结|
|module|模块|模组|
|template|模板|范本|
|text reference|文本引用|文字参考|
|operator|操作符/运算符|运算子|
|command|命令|指令|
|pragma|编译指令|编译指示|
|prefix|前缀|前置码|
|suffix|后缀|后置码|
||||

## see-also
- [TiddlyWiki — a non-linear personal web notebook](<https://tiddlywiki.com/>)
- [TiddlyWiki/Dev — documentation for developers](<https://tiddlywiki.com/dev/>)
- [TiddlyWiki 舞 — 基礎文件正體中文版](https://tw5-zh.tiddlyspot.com/)
- [TiddlyWiki — 非线性个人网络笔记本 (ver.5.1.15)](https://oss.hintsnet.com/mirror/tiddlywiki.cn.html)
  - [(http) TiddlyWiki — 非线性个人网络笔记本](http://oss.hintsnet.com/mirror/tiddlywiki.cn.html)
- [TiddlyWiki 舞 — 基础文档简体中文版 (github)](https://bramchen.github.io/tw5-docs/zh-Hans/)
  - [TiddlyWiki 舞 — 基础文档简体中文版 (tiddlyspot)](https://tw5-zh-hans.tiddlyspot.com/)
- [(http) TiddlyWiki 备忘录 — 官网副本中文版 • 2021年11月1日](http://tiddlywiki.cn/)
### sharing
- [Grok TiddlyWiki — Build a deep, lasting understanding of TiddlyWiki](https://groktiddlywiki.com/read/)
- [TiddlyWiki xp — A chance to experience TiddlyWiki very quickly](https://keatonlao.github.io/tiddlywiki-xp/)
### community

---
---
---
- Stamp
- [story]
  - SubStories
  - StoryView
    - StoryRiver
    - StoryList
- Titles Policy
- banner / Corner ribbon
- Upgrading
- (Working with TiddlyWiki)
  - PermaLink
  - 标签丸（tag pill）
  - 信息面板（InfoPanel）
    - 参照（References） [backlink]
    - 子条目（Tagging）
    - 列表（List） / 被列于（Listed） [field:list]
  - 边栏选项卡（sidebar tabs）
    - open recent more
  - search
  - journalTiddler
  - tagging
  - KeyboardShortcuts
  - Encryption
  - Audio
  - Performance
- (Customise TiddlyWiki)
  - custom sidebar button
  - StoryList
- Cascades
