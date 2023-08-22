---
title: "Fixing Workspaces Plus Plugin"
aliases:
  - 
tags:
  - snippet
date: 2023-08-15
---

From [this discussion](https://github.com/nothingislost/obsidian-workspaces-plus/issues/86) on github:

I found an easy fix, while we wait for [@nothingislost](https://github.com/nothingislost) to handle this properly:

-   Navigate to `<vault>/.obsidian/plugins/workspaces-plus/` and open `main.js`
-   find the following lines:

```javascript
// clone the input element as a hacky way to get ri
const inputElClone = this.inputEl.cloneNode();
this.modalEl.replaceChild(inputElClone, this.inputE
this.inputEl = inputElClone;
```

- comment out these lines

```javascript
// clone the input element as a hacky way to get ri
// const inputElClone = this.inputEl.cloneNode();
// this.modalEl.replaceChild(inputElClone, this.inp
// this.inputEl = inputElClone;
```