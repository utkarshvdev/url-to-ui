# 🖼️ Compositing and Layers – Final Frame Assembly

Compositing takes all the layers (bitmaps from paint phase) and assembles them on screen, using the **GPU** to accelerate the process.

## 🧩 Steps:
1. Divide painted content into layers
2. Use GPU to composite layers in correct order (z-index, opacity)
3. Output final frame to the screen

## 🖼️ GPU Accelerated Tasks:
- Transformations (e.g., `translate`, `scale`)
- Opacity changes
- Animations (e.g., `requestAnimationFrame`)

## 📊 Diagram:
```text
Painted Layers
  ↓
Compositor Thread (GPU)
  ↓
Final Frame
```

## ✅ Key Notes:
- Use `will-change` to promote to GPU layer
- Avoid unnecessary compositing (too many layers)
- Smooth UIs = efficient compositing + minimal reflows