---
layout: default
title: Smart Property
parent: Utilities
nav_order: 1
---

# Smart Property

Smart Property is an model and has some property.

```javascript
export class SmartProperty {
    key: string;
    title: string;
    smartHtml?: (item, key) => string;
    inlineSearch ?= false;
    searchable ?= true;
    visible ?= true;
    width?: string;
    type?: SmartDataTypes = SmartDataTypes.Text;
}
```

| Property  | Explanation                          |
|:----------|:-------------------------------------|
| `key`    | Key of one property of data  |
| `title`      | Title of one of column Ng Smart Table                  |
| `smartHtml`      | Column definition of property              |
| `inlineSearch`      |  Has column inlineSearchable (**default**: _false_)               |
| `visible`      | Is visible column (**default**:_true_)                |
| `width`      | Width of column              |
| `type`      | [SmartDataTypes]({{ site.baseurl }}{% link docs/types/data-type.md %}) (**default**:_Text_)              |

---

> Example SmartProperty

```javascript

colDef = (item, key) => {
    return `<div class="name-cell-column"><a href="${item[`${key}`]}">${item[`${key}`]}</a></div>`;
  }

model: SmartModel = {
    properties: [
      {
        title: 'NAME',
        key: 'Name',
        inlineSearch: true,
        smartHtml: this.colDef,
        width: '300px'
      }
      ...
    ]
};
```
