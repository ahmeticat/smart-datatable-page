---
layout: default
title: Add Click Event
parent: Events
nav_order: 1
---

> Ng Smart Datatable has some output events and one of these is btnAddClickEvent.

btnAddClickEvent is emit when ActionType.Add clicked.

This event can be listened like that

```javascript
(btnAddClickEvent)="btnAddClick()"
```

on .ts file

```javascript
btnAddClick() {
    console.log('BtnAdd Clicked');
}
```
