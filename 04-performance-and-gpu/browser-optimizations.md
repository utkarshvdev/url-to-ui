# 🚀 Browser Optimizations – Making UIs Fast and Fluid

Browsers employ several techniques to improve rendering performance and reduce visual jank.

## 🔧 Key Techniques:
1. **Layout Tree Caching**
2. **Style Recalculation Deduping**
3. **Offscreen Rendering**
4. **Partial Invalidation Painting**
5. **Lazy Loading and Deferral**

## 🧠 Critical Rendering Path (CRP):
- Optimizing the path from HTML/CSS/JS → Pixels
- Techniques: preload, async/defer scripts, font-display, etc.

## 🧪 DevTools Insights:
Use Chrome DevTools → Performance tab → Frames, Layers, Recalculate Styles

## ✅ Best Practices:
- Minimize layout shifts
- Reduce DOM depth
- Optimize paint-heavy elements (e.g., shadows, gradients)