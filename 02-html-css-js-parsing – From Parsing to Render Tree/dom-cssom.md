# 🧩 DOM + CSSOM → Render Tree

## 🔸 Combined Structure: Render Tree

- The DOM provides the structure
- The CSSOM provides the styles
- Together they form the Render Tree, which is used to paint pixels to the screen

---

## 🧠 Steps:

1. Parse HTML → DOM
2. Parse CSS → CSSOM
3. Merge DOM + CSSOM → Render Tree
4. Layout – Calculate position & size
5. Paint – Fill pixels
6. Composite – Render final frame to screen

---

## 📊 Diagram:

```text
HTML → DOM ┐
           ├─> Render Tree → Layout → Paint → Composite
CSS → CSSOM ┘
```

---

## ✅ Summary

- DOM + CSSOM = Render Tree
- Layout and painting are based on this tree
- Efficient rendering depends on minimizing reflows and repaints