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
    some()  //[any] \
    forEach() \
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
  
