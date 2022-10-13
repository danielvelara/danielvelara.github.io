---
title: "FastAPI Tutorial"
date: 2022-09-25T12:46:08-05:00
author: Daniel Velázquez
draft: false
tags: ["python", "fastapi"]
---

> FastAPI is a modern, fast (high-performance), web framework for building APIs with Python 3.7+ based on standard Python type hints.

![img](/img/fastapi.png)

## Hello World

```py {linenos=false,hl_lines=[1,"4-5"],linenostart=199}
from fastapi import FastAPI
app = FastAPI()

@app.get('/')
async def root():
    return {'message': 'Hello World'}
```
