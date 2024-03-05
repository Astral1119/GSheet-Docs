---
title: Query Arithmetic
tags:
  - technique
  - query
dg-publish: true
dg-permalink: query-arithmetic
---
[[QUERY|The QUERY function]] is able to process arithmetic functions by default, being processed on the same level as other data manipulation functions. As such, it allows for arithmetic processing via strings.
# Syntax
```xls
INDEX(QUERY(, "select "&expression, ), 2)
```

[[Code golf]] syntax for non-array-enabled formulae:

```xls
+SORT(QUERY(, "select "&expression, ))
```

* `expression` should be an arithmetic expression using only `+`, `-`, `*`,  and `/`. It should be submitted as a string.