---
cssclasses:
  - a4-page
UID:
tags:
  - Logs
highlight:
keywords:
archive-id:
protocols:
---

![[_Part_LogsChecker.base]]

# Title


```meta-bind-js-view
{highlight} as highlight
---
let highlight = context.bound.highlight;
if (!Array.isArray(highlight)) {
return "";
}

if (highlight.length === 0) {
return "";
}

// 直接返回处理结果
return highlight
.map((value, index) => `(${index + 1}) ${value}`)
.join("\n");
```

> **Keywords**: `VIEW[{keywords}][text]`

## Detail 1

## Protocols

![[_Logs2Protocols.base]]