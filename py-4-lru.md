- datetime.datetime.now().isoformat(sep, timespec)
- hashlib.sha1(:bytes)
  - update(:bytes)
  - hexdigest()
- iter(:func, :sentinel) [^ 1](https://docs.python.org/zh-cn/3/library/functions.html#iter)
  ```py
  from functools import partial
  with open('mydata.db', 'rb') as f:
    for block in iter(partial(f.read, 64), b''):
        process_block(block)
  ```
