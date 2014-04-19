---
title: "Terminology"
output:
  html_document: default
---

Networks have two main components, nodes and edges.

Nodes are the entities and esges are what connects them.



```r
library(igraph)

g <- graph.empty(n = 0)

g <- g + vertices(letters[1:3])

V(g)
```

```
## Vertex sequence:
## [1] "a" "b" "c"
```

```r
plot(g)
```

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-11.png) 

```r

g <- g + edges("a", "b", color = "red")

E(g)
```

```
## Edge sequence:
##     e       
## e [1] a -> b
```

```r
plot(g)
```

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-12.png) 

```r
g <- g + edges("b", "c", color = "red")

```


You can also embed plots, for example:

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 


Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
