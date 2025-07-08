# 📄 Render Tree – What is the Render Tree?

The **Render Tree** is created by combining the DOM (structure) and CSSOM (style). It contains only the visible nodes and the exact visual styles required to display them.

## 🧩 Steps:
1. Traverse the DOM
2. Skip nodes like `<script>`, `<meta>`, etc.
3. Apply computed styles from CSSOM
4. Create visual “render objects” for visible elements

## 📊 Diagram:
```text
DOM ─┐           
     ├─ + CSSOM → Render Tree
     └─ Invisible elements excluded
```

## ✅ Key Notes:
- Render tree is **not the same as DOM**
- Only visible elements are part of it
- Each node in render tree is a styled box