# bs4/beautifulsoup4
- (element/soup)
  - .childtag
    .contents
    .children{iter}
  - .string
    .strings
    .stripped_strings
  - select(:css)
    select_one
    find
    find_all
  - [:tag-attr]/get(:tag-attr)
    .:childtag-name
  - prettify 
    get_text(:sep, strip)
- BeautifulSoup(:src, :parser/markup)
- diagnose.diagnose()
# requests
- (response)
  - .text
    json()
    .request
    .raw
    .content
    .ok
    .reason
    .status_code
    .url
- (request)
  - Session()
  - Request() 
# feedparser
- parse(:src/url/str)
  - .feed
    - title
      link
      description
      published
      published_parsed
      updated
      cloud
  - .entries
    - content
      summary
      enclosures{attachments}
      contributors
      links
  - .channel
  - [items]
  - .namespaces
  - .version
  - .bozo{error}
