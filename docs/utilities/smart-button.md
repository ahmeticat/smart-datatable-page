---
layout: default
title: Smart Button
parent: Utilities
nav_order: 3
---

## Smart Button

Smart Button is an model and has some property.

```javascript
export class SmartButton {
    type: SmartButtonType;
    content: string;
    htmlClass?: string;
    visible: boolean;
    title?: string;
    action: () => void;
    buttons?: SmartButton;
}
```

| Property  | Explanation                          |
|:----------|:-------------------------------------|
| `type`    | ButtonType  |
| `content`      | html content of button                  |
| `visible`      | visibility of button              |
| `htmlClass`      | html class of button              |
| `action`      |  emittable click event when button click               |
| `buttons`      |  buttons of button               |

---

> Example SmartButton

```javascript

model: SmartModel = {
    properties: [
      ...
    ],
    buttons: [
      {
        content: 'Custom',
        type: SmartButtonType.Custom,
        visible: true,
        action: this.btnCustomButtonClick
      },
      {
        content: 'Custom Excel Button',
        type: SmartButtonType.Excel,
        visible: true,
        action: this.btnCustomExcelButtonClick
      }
    ]
};

btnCustomButtonClick() {
   console.log(`Custom Button Click`);
}

btnCustomExcelButtonClick() {
   console.log(`Custom Excel Button Click`);
}
```
