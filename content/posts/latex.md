---
title: "LaTeX"
date: 2022-09-26T17:54:46-05:00
author: Daniel Velázquez
math: true
draft: true
---

> You can embed KaTeX/LaTeX in Hugo

<script>
    document.addEventListener("DOMContentLoaded", function() {
        renderMathInElement(document.body, {
            delimiters: [
                {left: "$$", right: "$$", display: true},
                {left: "$", right: "$", display: false}
            ]
        });
    });
</script>

## Inline Math

Check out this equation $x = {-b \pm \sqrt{b^2-4ac} \over 2a}$ so cool!

## Math Block

$$
\iiint_{x-1}^{x+1}{f(x)dxdydz}
$$
