---
layout: default
title: Configuration
nav_order: 2
---

# Configuration
{: .no_toc }


**Ng Smart Datatable** has some specific configuration parameters that can be defined in model is implemented from SmartModel.
{: .fs-6 .fw-300 }

## Table of contents

1. [Properties](#properties)
2. [Actions](#actions)
3. [Buttons](#buttons)
4. [Language](#language)

```javascript
  export class SmartModel {
    properties: SmartProperty[];
    actions?: SmartAction[];
    buttons?: SmartButton[];
    language?: SmartLanguage;
  }
```

---

## Properties

Smart Model has a property which is properties implemented from SmartProperty

```javascript
properties: SmartProperty[]
```

## Actions

Smart Model has a property which is actions implemented from SmartAction

```javascript
actions: SmartAction[]
```

## Buttons

Smart Model has a property which is buttons implemented from SmartButton

```javascript
buttons: SmartButton[]
```

## Language

Smart Model has a property which is language implemented from SmartLanguage

```javascript
language: SmartLanguage[]
```
