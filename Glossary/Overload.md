---
title: Overload
tags: 
dg-publish: true
dg-permalink: overload
---
The `onEdit()` trigger can [only queue up to two trigger events](https://developers.google.com/apps-script/guides/triggers#:~:text=Note%3A%20The%20onEdit()%20trigger%20only%20queues%20up%20to%202%20trigger%20events.). When a user creates more trigger events than `onEdit()` can handle, it can miss inputs. This is known as overloading the trigger.