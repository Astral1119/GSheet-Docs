---
title: LAMBDA Recursion
tags:
  - technique
  - lambda
  - algorithms
dg-publish: true
dg-permalink: recursion
---
LAMBDA Recursion is a technique that uses a [[LAMBDA]] term that calls itself in order to perform recursion.
# Syntax
```xls
LET(func, LAMBDA(func, <variables>, <expression>), func(func, <variables>))
```

```xls
LAMBDA(func, func(func, <variables>))(LAMBDA(func, <variables>, <expression>))
```

Either syntax is valid; however, [[LET]] is typically easier to work with and read.