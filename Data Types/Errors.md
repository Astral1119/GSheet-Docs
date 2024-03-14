---
title: Errors
tags:
  - data-types
dg-publish: true
dg-permalink: errors
---
There are eight types of errors in Google Sheets. They are typically functionally equivalent, except for functions like `IFNA` or `ISERR`.
# Error Types
## \#NULL!
This error does not exist in Google Sheets naturally. It is listed due to compatibility with Excel, where \#NULL! results from an intersect operator which does not exist in Google Sheets.
## \#DIV/0!
\#DIV/0! results when one tries to divide by 0.
This error typically occurs when using /, but it can also occur when using AVERAGE and the like.
There are very few causes for this error, and so it is usually easy to point out what is causing it.
## \#VALUE!
\#VALUE! results when a function receives a data type it cannot handle, and that Google Sheets cannot coerce into one that it can.
You’ll likely have seen it quite a bit in the above sections on data types. Unfortunately, this also means that it can be difficult to figure out where issues arise.
Luckily, the error message will often say which function produces this error.
## \#REF!
\#REF! results from four different possibilities: missing reference, out of bounds, circular dependency, and expansion block.
1. Missing reference: If a cell gets deleted, all references to that cell will be replaced with \#REF!.
2. Out of bounds: A function attempts to retrieve an index of an array that does not exist.
3. Circular dependency: A function refers to the cell it is located in, or refers to a cell that is in any way affected by it.
4. Expansion block: A formula attempts to output an array but the array cannot expand due to being blocked by another value or the edge of the sheet.
Be careful of array expansion when you get to array formulae. If there are missing rows, Google Sheets will attempt to create up to 50,000 new rows.
## \#NAME?
\#NAME? results from trying to call a nonexistent function or range.
## \#NUM!
\#NUM! results from submitting an invalid number to a function. For example, attempting to take the square root of a negative number or attempting to find the n + 1th smallest number in a set of numbers of size n.
## \#N/A
\#N/A signifies that the formula has successfully executed, but that valid results were not available.
This error commonly results from lookup functions or FILTER. It is typically expected, and resolved using IFNA.
## \#ERROR!
If Google Sheets is unable to parse your formula, it will return \#ERROR!.
Missing parentheses and typos are frequent culprits.
# Behavior
Most formulae, if given an error, will halt calculations and return the same error it was given; in this way, errors can ‘carry forward.’ This is very useful for debugging, but also means that they must be actively managed using functions such as `IFERROR`.

However, note that some functions do not carry errors forward. For example, `COUNTA` will count errors just the same as any other value.