

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
- [query]
### HTMLDocument
### DocumentFragment (Node)
- [tree]
- [query]
- [init]
  - document.createDocumentFragment()
  - new DocumentFragment()
### DOMParser
### XPathEvaluator

## Window

## web-api
### WebRTC
### WebGL
### wasm
### Web Speech API
