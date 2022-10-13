---
title: "Hugo Tutorial"
author: Daniel Velázquez
date: 2022-09-25

draft: false
---

## Other Elements — abbr, sub, sup, kbd, mark

[^1]: This is not a lie

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

# H1

## H2

### H3

#### H4

##### H5

| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |

This is a lie [^1]
[^1]: This is not a lie

```py
from fastapi import FastAPI
app = FastAPI()

@app.get('/')
async def root():
    return {'message': 'Hello World'}
```

```go {linenos=false,hl_lines=[1,"4-5"],linenostart=199}
package main

import (
    "fmt"
    "net/http"
    "time"
)

func greet(w http.ResponseWriter, r *http.Request) {
    fmt.Fprintf(w, "Hello World! %s", time.Now())
}

func main() {
    http.HandleFunc("/", greet)
    http.ListenAndServe(":8080", nil)
}
```

Term
: Definition

## Shortcodes

### YouTube Privacy Enhanced Shortcode

{{< youtube ZJthWmvUzzc >}}

### Caption

{{< figure src="/img/doge.png" title="Doge Coin" >}}

![Doge](/img/doge.png)

### GitHub gist

{{< gist spf13 7896402 >}}

### Twitter

{{< tweet user="SanDiegoZoo" id="1453110110599868418" >}}
