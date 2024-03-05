---
title: Calculation Limits
tags:
  - technique
dg-publish: true
dg-permalink: written-numbers
---
Google Sheets does not natively support a way to convert numbers into their [written form](https://en.wikipedia.org/wiki/English_numerals). However, by using the `BAHTTEXT` function in conjunction with `GOOGLETRANSLATE` we can approximate a written form.
# Syntax
```xls
SUBSTITUTE(GOOGLETRANSLATE(BAHTTEXT([number])), " baht", )
```
# Notes
* The efficacy of this technique is dependent on the accuracy of Google Translate. As Google Translate is error-prone, so too is this technique.
* It typically fails with larger numbers.