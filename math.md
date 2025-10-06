# Introduction
You can include any mathematical expression supported by [MathJax](https://www.mathjax.org/) within a workflow. Mathematical expressions can be added to the Markdown content in a manner similar to [Github](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions).

## Block Expressions
You can define the start and end of mathematical blocks with `$$`. 
For example `$$ \left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right) $$` will be rendered as:\
$$ \left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right) $$ 

tetstsd

Make sure to include a space between the `$$` and the mathematical expression(s).

This also works with:
```
$$
\sqrt{\$4}
$$
```

$$
\sqrt{\$4}
$$

Alternatively you can use `math` blocks:
````
``` math
\sqrt{3x-1}+(1+x)^2
```
````

``` math
\sqrt{3x-1}+(1+x)^2
```

## Inline Expressions
Inline mathematical expressions are also supported. Use a single `$` to start and finish a mathematical expression inside a text. For example `$(ax^2 + bx + c = 0)$` will render to $(ax^2 + bx + c = 0)$. 
You can also use ``$`...math`$``, e.g. ``$`x = {-b \pm \sqrt{b^2-4ac} \over 2a}`$`` will result in $`x = {-b \pm \sqrt{b^2-4ac} \over 2a}`$.

## The \$ Special Character
As `$` is used to detect the bounds of a mathematical expression, you have to escape it with `\` to specify \$ inside an expression: `\$`.
