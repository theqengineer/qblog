---
title: python
published: 2026-03-03
description: ''
image: ''
tags: []
category: ''
draft: false 
lang: ''
---

[@overload](https://docs.python.org/zh-cn/3.14/library/typing.html#typing.overload)

```py
from typing import overload

@overload
def process(response: None) -> None:
    ...
@overload
def process(response: int) -> tuple[int, str]:
    ...
@overload
def process(response: bytes) -> str:
    ...
def process(response):
    ...  # 以下为真正的实现
```

```py
    def get_next(
        self, *, format: ResultFormat = ResultFormat.AUTO
    ) -> t.Union[GroupResult, Result]:
```