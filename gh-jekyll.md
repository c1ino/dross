- _posts / post
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
- _drafts
- pages
- _layouts / [Layouts | Jekyll](https://jekyllrb.com/docs/layouts/)
  - default.html
  - [font-matter]
    - [Inheritance]
    - [Variables] layout
- _config.yml
  - defaults / [Front Matter Defaults | Jekyll](https://jekyllrb.com/docs/configuration/front-matter-defaults/)
  - permalink / [Permalinks | Jekyll](https://jekyllrb.com/docs/permalinks/)
    - `/:categories/:year/:month/:day/:title:output_ext`
  - [collections] / [Collections | Jekyll](https://jekyllrb.com/docs/collections/)
    - collections
      - :name
        - output: `true`
        - order
        - sort_by 
    - collections_dir: my_collections
  - page_excerpts: `true`
  - layouts_dir
  - plugins
  - theme
  - [paginate] / [Pagination | Jekyll](https://jekyllrb.com/docs/pagination/)
    - paginate
    - paginate_path: `"/blog/page:num/"`
  - [flags]
    - show_drafts unpublished future
  - [Default Configuration | Jekyll](https://jekyllrb.com/docs/configuration/default/)
- assets
- index.html/md
### misc
- _data
- _includes / [Includes | Jekyll](https://jekyllrb.com/docs/includes/)
- _sass
- _site
### theme
- [Themes | Jekyll](https://jekyllrb.com/docs/themes/)
- [Supported themes | GitHub Pages](https://pages.github.com/themes/)


## Liquid
### grammar
- {{ variable }}
- {% if statement %}
- tags
- filters
- [Jekyll Cheat Sheet | CloudCannon](https://cloudcannon.com/community/jekyll-cheat-sheet/)
### jekyll
- [include]
  - {% include footer.html %}
  - {% include_relative somedir/footer.html %}
  - {% include {{ page.my_variable }} %}
  - {{ include.content }}
- [layout]
  - {{ content }}
  - page 

## github-pages
- [关于 GitHub 页面和 Jekyll - GitHub Docs](https://docs.github.com/zh/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)
- [Using site.github | GitHub Metadata](https://jekyll.github.io/github-metadata/site.github/)
