## Array
- [init]
  - from(:iter)
  - Array(:len) Array(...items)
  - of(...items)
  - concat(arr1, ...)
- [iter]
  - entries() keys() values() 
  - for(let item of array){}
- [get]
  - slice() at(:pos)
- [String]
  - join() 
- [fp]
  - every()  //[all] \
    some()  //[any]
  - forEach() \
    map() \
    filter() \
    reduce() reduceRight()
  - flat() flatMap()
  - group() groupToMap()
- [find]
  - includes()
    indexOf() lastIndexOf() \
    find() findIndex() findLast() findLastIndex()
- [set]
  - pop() push()
    sort() reverse()
    shift() unshift() \
    splice(:start, :len, ...ins_items) 
  - copyWithin(:dst, :strat, :end) \
    fill(:val, :start, :end)
- isArray() valueOf() toString() toLocaleString() length

## String
- [array]
  - concat()
  - indexOf() includes()
  - slice() at() length
- [Array]
  - split()
- [str]
  - trim() trimStart() trimEnd() //[strip]
  - charCodeAt() fromCharCode() codePointAt() fromCodePoint()
  - endsWith() startsWith()
  - repeat() padEnd() padStart()
  - charAt() substr() substring()
  - toLowerCase() toUpperCase() toLocaleLowerCase() toLocaleUpperCase()
  - localeCompare()
  - normalize()
  - raw()
- [regex]
  - search() match() matchAll() 
  - replace() replaceAll()
- [html]

## RegExp
- [init]
  - /regex/flag
  - new RegExp(:regex, :flag)
- [attr]
  - [flags]
- [regex]
  - compile()
  - test() exec()

## Object
- [oop]
  - prototype [[proto]] constructor
- [init]
  - [literal]
  - create(:proto, :props_obj)
- [set]
  - assign(:dst, ...src)  //[extend/update]
  - setPrototypeOf()
- [prop]
  - defineProperty() defineProperties()
  - getOwnPropertyDescriptor()
  - getOwnPropertyNames() getOwnPropertySymbols()
  - freeze() seal() preventExtensions()
  - hasOwnProperty()
  - propertyIsEnumerable()
  - delete
- [get]
  - entries() keys() values()
  - getPrototypeOf()
- [misc]
  - is() isExtensible() isFrozen() isSealed()
  - isPrototypeOf()
  - valueOf()
- [str]
  - toString() toLocaleString()

### prop descriptor
- configurable
- enumerable
- value writable
- get set
#### accessor

---
---
---
- Symbol
- Map Set WeakMap WeakSet
- Date
- Function
- Proxy Reflect
- Number Math
