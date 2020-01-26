---
layout: default
title: Smart Action
parent: Utilities
nav_order: 2
---

# Smart Action

Smart Action is an model and has some property.

```javascript
export class SmartAction {
    type: ActionType;
    content: string;
    visible: boolean;
    click?: (item) => void;
}
```

| Property  | Explanation                          |
|:----------|:-------------------------------------|
| `type`    | [ActionType]({{ site.baseurl }}{% link docs/types/action-type.md %})   |
| `content`      | html content of action                  |
| `visible`      | visibility of action              |
| `click`      |  emittable click event when action click               |

---

> Example SmartAction

```javascript

model: SmartModel = {
    properties: [
      ...
    ],
    ...,
    actions: [
      {
        type: ActionType.Add,
        content: '<input type="button" value="Add" class="add-item">',
        visible: true
      },
      {
        type: ActionType.Custom,
        content: 'First Custom Button',
        visible: true,
        click: this.btnCustomClick
      },
      ...
    ]
};

btnCustomClick(item: any) {
    console.log(`Custom Action Click : ${JSON.stringify(item)}`);
}
```
