## Array
- [init]
  - from(:iter)
  - Array(:len) Array(...items)
  - of(...items)
- [iter]
  - entries() keys() values() 
  - for(let item of array){}
- [get]
  - slice() at(:pos)
- [basic]
  - join() concat()
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
- [basic]
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
- [regex]
  - match() matchAll() search()
  - replace() replaceAll()
- [html]
