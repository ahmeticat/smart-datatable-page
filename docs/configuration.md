---
layout: default
title: Configuration
nav_order: 2
---

# Configuration
{: .no_toc }

**Ng Smart Datatable** has some specific configuration parameters that can be defined in model is implemented from SmartModel.
{: .fs-6 .fw-300 }


```javascript
  export class SmartModel {
    properties: SmartProperty[];
    actions?: SmartAction[];
    buttons?: SmartButton[];
    language?: SmartLanguage;
  }
```

---

### Properties

Smart Model has a property which is properties implemented from [SmartProperty]({{ site.baseurl }}{% link docs/utilities/smart-property.md %})


```javascript
properties: SmartProperty[]
```

### Actions

Smart Model has a property which is actions implemented from [SmartAction]({{ site.baseurl }}{% link docs/utilities/smart-action.md %})

```javascript
actions: SmartAction[]
```

### Buttons

Smart Model has a property which is buttons implemented from [SmartButton]({{ site.baseurl }}{% link docs/utilities/smart-button.md %})

```javascript
buttons: SmartButton[]
```

### Language

Smart Model has a property which is language implemented from [SmartLanguage]({{ site.baseurl }}{% link docs/utilities/smart-language.md %})

```javascript
language: SmartLanguage[]
```
