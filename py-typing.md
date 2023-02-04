- Any
- NoReturn
- TypeAlias ((3.10+))
###
- Tuple[X, Y, ...] ((3.9-))
- Union[X, Y, ...] ((3.10+ `X|Y|...`))
  - Optional[X]
  - Literal[x, y, ...] ((3.8+))
    - Final ((3.8+)) ((constant))
- Callable[[ParamType, ...], ReturnType] ((3.9-))
  - Concatenate[Arg1Type, Arg2Type, ..., ParamSpecVariable] ((3.10+))
- Type[C] ((3.9-))
- ClassVar
- Annotated ((3.9+))
- TypeGuard ((3.10+))
###
- Generic
- TypeVar
- ParamSpec ((3.10+))
- AnyStr
- Protocol ((3.8+))
###
- NamedTuple
- NewType
- TypedDict ((3.8+))
### ((3.9-))
- Dict, List, Set, FrozenSet
- collections
  - DefaultDict, OrderedDict, ChainMap, Deque
- collections.abc

---
---
---
- PEP 3107 – Function Annotations
- PEP 484 483
