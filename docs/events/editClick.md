---
layout: default
title: Edit Click Event
parent: Events
nav_order: 2
---

> Ng Smart Datatable has some output events and one of these is btnEditClickEvent.

btnEditClickEvent is emit item when [ActionType]({{ site.baseurl }}{% link docs/types/action-type.md %}).Edit clicked.

This event can be listened like that

```javascript
(btnEditClickEvent)="btnEditClick($event)"
```

on .ts file

```javascript
btnEditClick(item: any) {
    console.log(`Edit Click : ${JSON.stringify(item)}`);
}
```
