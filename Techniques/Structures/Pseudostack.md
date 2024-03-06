---
dg-publish: true
tags:
  - structures
dg-permalink: pseudostack
---
The pseudostack is a virtual structure that uses [[Arrays]] to simulate a [stack](https://en.wikipedia.org/wiki/Stack_(abstract_data_type)). Unlike a true stack, the pop operation cannot be used to read the first-out value. Therefore, peek must be used prior to pop. Because [[query]] requires homogenous data types, pseudostacks are string-only structures.
All three operations are comparatively efficient. Applications of this structure are rare and typically occur in [[algorithmic formulae]].
# Operations

# Push
```xls
{<string>; pstack}
```

# Pop
```xls
query(pstack, "offset 1",)
```

# Peek
```xls
single(pstack)
```