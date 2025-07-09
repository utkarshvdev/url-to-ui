# 🧱 Layers and GPU Acceleration – Promoting Smooth UIs

Modern browsers use the GPU for compositing layers and optimizing rendering performance.

## 🎯 What are Layers?
Browser breaks up content into layers that can be individually painted and composited.

### Triggering Layers:
- `will-change`
- `transform`, `opacity`, `filter`
- CSS animations

## ⚙️ GPU Compositing:
Once painted, layers are handed off to the GPU, which handles:
- Z-index stacking
- Transformations
- Opacity transitions
- Frame rendering

## ✅ Tips:
- Promote frequently changing elements to layers
- Use `will-change: transform;` sparingly
- Avoid over-promotion (too many layers hurt memory)