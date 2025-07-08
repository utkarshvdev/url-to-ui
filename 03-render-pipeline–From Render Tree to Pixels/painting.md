# 🎨 Painting – Filling Pixels with Colors

Painting is the process of filling in **pixels** for visual parts of the layout – text, images, borders, shadows, backgrounds.

## 🧩 What Happens:
1. Translate layout boxes into pixel instructions
2. Break each visual into **painting layers**
3. Store results in a bitmap (rasterization)

## 🧠 Includes:
- Color fills, shadows
- Fonts, borders
- Gradients, images

## 📊 Diagram:
```text
Layout Tree
  ↓
Display Items (Paint Instructions)
  ↓
Bitmaps (Per Layer)
```

## ✅ Key Notes:
- Paint can be optimized using layer promotion
- CSS changes like color/border cause repaint