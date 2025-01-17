---
title: Fluid typography
tags: visual
expertise: intermediate
author: chalarangelo
firstSeen: 2021-05-16T11:23:05+03:00
lastUpdated: 2021-05-16T11:23:05+03:00
---

Creates text that scales according to the viewport width.

- Use the `clamp()` CSS function to clamp the value of `font-size` between `1rem` and `3rem`.
- Use the formula `8vw - 2rem` to calculate a responsive value for `font-size` (`1rem` at `600px`, `3rem` at `1000px`).

```html
<p class="fluid-type">Hello World!</p>
```

```css
.fluid-type {
  font-size: clamp(1rem, 8vw - 2rem, 3rem);
}
```
