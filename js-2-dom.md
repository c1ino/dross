

## EventTarget
- addEventListener
- removeEventListener
- dispatchEvent

## Node
- [tree]
  - childNodes firstChild lastChild
  - nextSibling previousSibling
  - parentNode parentElement
  - appendChild() removeChild() replaceChild()
  - insertBefore(:ins, :bef)
  - compareDocumentPosition()
  - contains() hasChildNodes()
  - getRootNode()
- [node]
  - nodeName nodeType
  - textContent
  - cloneNode()
  - isEqualNode() isSameNode()
  - normalize()
- [misc]
### NodeList

## Element
- [tag]
  - innerHTML outerHTML
  - localName tagName
- [attribute]
  - attributes
  - classList className
    - add() remove() replace() toggle()
  - getAttribute() getAttributeNames()
    hasAttribute() hasAttributes()
    removeAttribute()
    setAttribute()
    toggleAttribute()
- [tree]
  - nextElementSibling previousElementSibling
  - children childElementCount 
  - insertAdjacentElement(:pos, :el) 
    insertAdjacentHTML()
    insertAdjacentText()
  - append() prepend() before() after() remove()
  - replaceChildren() replaceWith()
- [event]
- [query]
- [screen]
  - [scroll]
  - [coordinate]
### DOMTokenList

## HTMLElement
- [tag]
  - innerText outerText
  - style
  - tabIndex
- [input]
  - focus blur click
- [misc]
  - contentEditable dataset draggable hidden offset style tabIndex
### HTMLCollection

## Events
- touch
- mouse
- keyboard
- fullscreen
- focus
- composition
- clipboard
- misc
  - cancel error scroll select show wheel

## URL
- [object-url]
- [init]
- [parts]
  - searchParams
### URLSearchParams
## Document (Node)
- [create]
- [tree]
  - activeElement head body
  - open() close() write()
  - forms images links scripts
- [query]
- [info]
  - baseURI domain referrer title URL documentURI
  - doctype inputEncoding lastModified readyState
  - cookie
### HTMLDocument
### DocumentFragment (Node)
- [tree]
- [query]
- [init]
  - document.createDocumentFragment()
  - new DocumentFragment()
### DOMParser
### XPathEvaluator

## Window / global
- [main]
  - document
    - defaultView  
  - location
  - history
  - navigator
  - console
  - localStorage sessionStorage
- [create]
- [tree]
  - top self window frames length opener parent
  - open() close()
- [web-api]
- [input]
  - alert confirm prompt
  - blur focus
  - getSelection()
- [event]
- [state]
  - event 
  - stop()
- [info]
  - name origin href
- [screen]
  - screen
  - visualViewport
- [util]
  - atob() btoa()
  - crypto
  - fetch()
  - setTimeout() setInterval()
    clearTimeout() clearInterval()
- [widget]
- [render]
- [misc]
### location
- assign() replace() reload()
- href protocol host hostname port pathname search hash username password origin

## web-api
### WebRTC
### WebGL
### WebSocket
### WebAssembly JavaScript API
### Web Speech API
### Web MIDI API
### Canvas API
### Encrypted Media Extensions API
