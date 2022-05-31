(3.7+) (for-asyncio)
- Context: Mapping
  - run(:func, *args, **kwrds)
    - enter context(self) for func
  - [:name] -> ContextVar
  - get(:name, :fallback) -> context[:name].get(:fallback)
  - copy() keys() values() items()
- copy_context() -> Context ((snapshot))
- ContextVar(:name, :val) ((must-global))
  - get(:fallback)
  - set(:val) -> Token
  - reset(:token)
- Token \<- ContextVar().set()


[MagicStack/contextvars: PEP 567 Backport]:(https://github.com/MagicStack/contextvars)
[如何使用contextvars模块和源码分析 - 掘金]:(https://juejin.cn/post/6975780543661260813)
