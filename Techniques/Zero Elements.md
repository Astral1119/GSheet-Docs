---
title: Zero Elements
tags:
  - data-types
  - technique
dg-publish: true
dg-permalink: zero-elements
---
Zero elements are values that, when used in an [[Arrays|array]], have no width and/or height. 
# Syntax
| **0 x 1** | **1 x 0** | **0 x 0** |
| :--: | :--: | :--: |
| `TOCOL(,1)` | `TOROW(,1)` | `ARRAY_CONSTRAIN(,,)` |
These zero elements can be useful when used in [[REDUCE]] or [[LAMBDA Recursion]] when used as an initial value. In some situations, a zero element can essentially remove an initial value from the accumulator.