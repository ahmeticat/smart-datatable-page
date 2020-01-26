---
layout: default
title: Delete Click Event
parent: Events
nav_order: 3
---

> Ng Smart Datatable has some output events and one of these is btnDeleteClickEvent.

btnDeleteClickEvent is emit item when [ActionType]({{ site.baseurl }}{% link docs/types/action-type.md %}).Delete clicked.

This event can be listened like that

```javascript
(btnDeleteClickEvent)="btnDeleteClick($event)"
```

on .ts file


```javascript
btnDeleteClick(item: any) {
    console.log(`Delete Click : ${JSON.stringify(item)}`);
}
```
