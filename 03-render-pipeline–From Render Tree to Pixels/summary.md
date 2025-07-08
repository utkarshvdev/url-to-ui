# 📘 Summary – Module 3: Render Pipeline

This module covers the final transformation of parsed content into pixels on the user's screen. It explains how the browser builds the render tree and executes layout, painting, and compositing.

---

## 📂 Topics Covered:

### 1. Render Tree (`render-tree.md`)
- Combines DOM + CSSOM
- Excludes invisible elements
- Builds styled visual boxes

### 2. Layout (`layout.md`)
- Computes position & size of elements
- Handles box model, flow, flex/grid
- Costly operation – optimize when possible

### 3. Painting (`painting.md`)
- Draws visual parts: colors, borders, text, shadows
- Produces bitmaps
- Affected by style changes

### 4. Compositing (`compositing-and-layers.md`)
- Uses GPU to assemble layers
- Handles z-index, transforms, animations
- Outputs final frame to screen

---

## ✅ Key Takeaways:

- Efficient rendering relies on optimized layout and minimal repaints.
- Paint & composite stages are GPU-accelerated.
- Understanding this pipeline helps in performance tuning and animation handling.