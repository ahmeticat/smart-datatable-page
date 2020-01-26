---
layout: default
title: Language
parent: Utilities
nav_order: 4
---


## Smart Language

Smart Language is an model and has some property.

```javascript
export class SmartLanguage {
    actionsColumnHeader?: string;
    lengthMenu?: string;
    search?: string;
    searchPlaceholder?: string;
    info?: string;
    filteredInfo?: string;
    paginationPrevious?: string;
    paginationNext?: string;
}
```

| Property  | Explanation                          |
|:----------|:-------------------------------------|
| `actionColumnHeader`    | html content of action column header   |
| `lengthMenu`      | html content of length menu                   |
| `search`      | html content of filter               |
| `searchPlaceholder`      |  placeholder of filter input                |
| `info`      | html content of info               |
| `filteredInfo`      | html content of filteredInfo               |
| `paginationPrevious`      | content of previous pagination button                |
| `paginationNext`      | content of next pagination button                |

---

> Example SmartLanguage

```javascript

model: SmartModel = {
    properties: [
      ...
    ],
    language: {
        actionsColumnHeader: 'Actions',
        filteredInfo: '(Filtered from **TOTAL** entries)',
        info: 'Showing **START** to **END** of **TOTAL** entries',
        lengthMenu: 'Show **LENGTH** entries',
        paginationNext: 'Next',
        paginationPrevious: 'Previous',
        search: 'Search : **SEARCH**',
        searchPlaceholder: 'Search'
    }
};
```
