- _posts / [Posts | Jekyll](https://jekyllrb.com/docs/posts/)
  - YEAR-MONTH-DAY-title.MARKUP
  - front-matter / [Front Matter | Jekyll](https://jekyllrb.com/docs/front-matter/)
    - layout
    - title
    - permalink
    - published
    - date: `YYYY-MM-DD HH:MM:SS +/-TTTT`
    - category categories
    - tags
    - excerpt_separator: `<!--more-->`
  - [*categories/_posts/]
- _drafts/
- [/page.ext] / [Pages | Jekyll](https://jekyllrb.com/docs/pages/)
- _layouts / [Layouts | Jekyll](https://jekyllrb.com/docs/layouts/)
  - default.html
  - [font-matter]
    - [Inheritance]
    - [Variables] layout
- _config.yml / [Configuration Options | Jekyll](https://jekyllrb.com/docs/configuration/options/)
  - defaults / [Front Matter Defaults | Jekyll](https://jekyllrb.com/docs/configuration/front-matter-defaults/)
    - scope:
      - path: "" / "dir"
        - "dir/*/globfile" ((3.7.0))
      - type: posts / pages / drafts / [collection]
    - values:
      - [font-matter]:
  - permalink / [Permalinks | Jekyll](https://jekyllrb.com/docs/permalinks/)
    - `/:categories/:year/:month/:day/:title:output_ext`
  - [collections] / [Collections | Jekyll](https://jekyllrb.com/docs/collections/)
    - collections
      - :name
        - output: `false`
        - order
        - sort_by 
        - permalink / [Permalinks | Jekyll](https://jekyllrb.com/docs/permalinks/#collections)
        - [font-matter]
    - collections_dir: `my_collections`
  - page_excerpts: `true`
  - layouts_dir
  - plugins
  - theme remote_theme
  - [paginate] / [Pagination | Jekyll](https://jekyllrb.com/docs/pagination/)
    - paginate
    - paginate_path: `"/blog/page:num/"`
  - [flags]
    - show_drafts unpublished future
  - include exclude
  - csv_reader tsv_reader / [Data Files | Jekyll](https://jekyllrb.com/docs/datafiles/#csvtsv-parse-options)
  - [Default Configuration | Jekyll](https://jekyllrb.com/docs/configuration/default/)
- assets/
- index.html index.md
- [_collection/]
  - [default-config.yml]
    - output: false

### misc
- _data
- _includes / [Includes | Jekyll](https://jekyllrb.com/docs/includes/)
- _sass
- _plugins / [Plugins | Jekyll](https://jekyllrb.com/docs/plugins/)
  - [generator]
  - [convertor]
  - [command]
  - [tag]
  - [filter]
  - [hook]
- _site

### theme
- [Themes | Jekyll](https://jekyllrb.com/docs/themes/)
- [Supported themes | GitHub Pages](https://pages.github.com/themes/)



## Liquid


### jekyll
- [variable]
  - site
    - pages posts documents
    - collections categories tags
      - collections / [Collections | Jekyll](https://jekyllrb.com/docs/collections/#collections)
        - label docs directory output
    - data
    - [_config.yml]
    - [meta]
  - page
    - collection tags category categories
    - path dir name 
    - url id date
    - next previous
    - title content excerpt
    - [page.font-matter]
  - layout
  - theme
  - [misc]
    - paginator
    - content
- [include]
  - {% include footer.html %}
  - {% include_relative somedir/footer.html %}
  - {% include {{ page.my_variable }} %}
  - {{ include.content }}
- [layout]
  - {{ content }}
  - page 


### grammar
- {{ variable }}
- {% if statement %}
- tags
- filters
- [Jekyll Cheat Sheet | CloudCannon](https://cloudcannon.com/community/jekyll-cheat-sheet/)
#### cheatsheet
- `{{ expr }}`
  - `{{ var | filter: arg1, ... | ... }}`
- `{% stmt/tag %}`
  - `{%- autostrip -%}`
  - [flow]
    - if unless elsif else 
    - case when
  - [iter]
    - for else break continue
      - limit: offset: range reversed
      - {{forloop}}
    - cycle
    - tablerow
  - [var]
    - assign
    - capture
    - increment decrement
  - [template]
    - comment {% # ...%}
    - raw
    - liquid echo
    - render (include)
- [type]
  - String
    - [truthy]
  - Number
    - [truthy]
  - Boolean
    - true false
  - Nil
    - [no-literal] [falsy]
    - (undefined/not-exist)
  - Array[index]
    - [no-literal] [truthy]
  - Object.key
    - [no-literal] [truthy]
  - EmptyDrop 
    - [no-literal] [truthy]
  - empty
    - [truthy]
    - (empty-array/string)
- [operator]
  - == != or and contains



## simple
- [_collections]
  - _posts _drafts
    - :date :categories
  - pages _collection
    - :basename
- [categories/page], [categories/_posts]
- _layouts _includes
  - _layouts
    - default
      - page
      - post
- _config.yml
- _data _plugins
### [type]
- dynamic/render
  - pages
  - collection/documents
    - posts drafts  
- static/resource
  - static_files
### [code]
- compile-time
  - liquid - template
  - ruby - plugin
- runtime
  - js - client


## github-pages
- [关于 GitHub 页面和 Jekyll - GitHub Docs](https://docs.github.com/zh/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)
- [Using site.github | GitHub Metadata](https://jekyll.github.io/github-metadata/site.github/)
- [Dependency versions | GitHub Pages](https://pages.github.com/versions/)

