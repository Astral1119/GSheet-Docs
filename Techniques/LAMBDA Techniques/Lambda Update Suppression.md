---
title: LAMBDA Update Suppression
tags:
  - technique
  - lambda
  - algorithms
dg-publish: true
dg-permalink: lus
---
LAMBDA Update Suppression (LUS) is an [[unstable]] technique that uses [[LAMBDA]] to prevent [[volatile functions]] from updating.
# Syntax
```xls
LAMBDA(volatile, update, volatile)([volatile function], [update condition])`
```

LAMBDA references only recalculate when a change is detected in a cell referenced by the formula. This property overrides the typical volatile property of updating whenever *any* cell is updated.

Because LUS is unstable, typical use cases relate to temporary randomization and dice rolling.