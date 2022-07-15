- logging
  - getLogger(:name) -> Logger
    - propagate, setLevel
    - getChild, findCaller
    - debug, info, warning, error, critical, exception, log
      - [10, 20, 30, 40, 50]
    - addFilter/removeFilter, filter
    - addHandler/removeHandler/hasHandlers, handle
  - (Handler)
  - Formatter
  - Filter
  - set/getLogRecordFactory() -> (LogRecord)
  - LoggerAdapter(:logger, :extra)
  - disable(level=CRITICAL)
  - addLevelName(level, levelName), getLevelName
  - basicConfig()
    - stream/filename filemode 
      - ((3.9+)) encoding errors 
    - format datefmt style
    - level handlers
    - force ((3.8+))
  - shutdown
- logging.handlers
- logging.config
  - fileConfig dictConfig

###
- level, logger, msg
  - msg
    - format, style
  - logger ((input))
    - filter ((process))
    - handler ((output))
      - formatter
####
[-]:https://docs.python.org/zh-cn/3/howto/logging.html#useful-handlers
