# 📘 Summary – Module 4: Performance and GPU

This module explores how browsers optimize rendering by minimizing layout and paint costs and leveraging GPU acceleration.

---

## 📂 Topics Covered:

### 1. Reflow vs Repaint
- Reflow: Layout recalculations, expensive
- Repaint: Appearance-only updates
- Avoid unnecessary layout changes

### 2. Layers and GPU Acceleration
- GPU compositing for smoother animations
- Layer promotion via transform, opacity, will-change
- Avoid layer abuse to prevent memory issues

### 3. Browser Optimizations
- Partial painting, layer reuse, style deduping
- Use of Chrome DevTools for analysis
- Tuning the Critical Rendering Path

---

## ✅ Takeaways:
- Understand what triggers reflows/repaints
- Use GPU wisely for performance gains
- Audit performance using DevTools
