# 📄 Layout – Positioning Elements on the Page

The layout stage computes the **position and size** of each object in the render tree.

## 🧩 Steps:
1. Start from the root (e.g., `<html>`, `<body>`)
2. Traverse recursively and calculate dimensions
3. Consider flow, box model, flex/grid rules

## 📦 Box Model Influence:
- `margin`, `padding`, `border`, `width`, `height`
- Layout is affected by fonts, images, screen size

## 📊 Diagram:
```text
Render Tree
  ↓
Layout Tree with size + coordinates
```

## ✅ Key Notes:
- A layout is triggered by DOM/CSSOM changes
- Costly operation (especially on large trees)
- Use `will-change` and `contain` wisely to optimize