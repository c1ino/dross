- logging
  - getLogger(:name) -> Logger
    - setLevel, [propagate]
    - debug, info, warning, error, critical, exception, log
      - [10, 20, 30, 40, 50]
    - getChild, findCaller
    - addFilter/removeFilter, filter
    - addHandler/removeHandler/hasHandlers, handle
  - addLevelName(level, levelName), getLevelName
  - disable(level=CRITICAL)
  - basicConfig()
    - stream/filename filemode 
      - ((3.9+)) encoding errors 
    - format datefmt style
    - level handlers
    - force ((3.8+))
  - shutdown()
  - ((class/factory))
    - Logger
      - set/getLoggerClass()
    - (Handler)
    - Formatter
      - asctime created msecs relativeCreated
      - args exc_info msg stack_info
      - pathname/filename module funcName 
      - message name levelname/levelno 
      - process/processName thread/threadName
    - Filter
    - LogRecord
      - set/getLogRecordFactory() -> (LogRecord)
      - makeLogRecord()
    - LoggerAdapter(:logger, :extra)
- logging.handlers [^ 1]
- logging.config
  - fileConfig dictConfig

[^ 1]:https://docs.python.org/zh-cn/3/howto/logging.html#useful-handlers

###
- level, logger, msg
  - msg
    - format, style
    - (level)
  - logger ((input))
    - filter ((process))
    - handler ((output))
      - formatter ((template))
      - (level)
    - (level)
####
[max]:1
